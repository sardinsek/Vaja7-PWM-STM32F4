# Vaja7-PWM-STM32F4
Prvi kanal sva aktivirala kot PWM Generation CH1. Omogočila sva pin PE9. Poleg njega pa se izpiše oznaka TIM1_CH1.
Vrednost Perscaler sva nastavila na 16.
Parameter Counter Period sva nastavila na 100 in s tem še dodatno znižala takt časovnika. Takt sedaj znaša 10 kHz.
V PWM Generation Chanel sva nastavila Pulse (16 bits value) na 50. Ta parameter pomeni, da delovni cikel deluje na 50 % svoje zmogljivosti.
V kodi sva spremenila vrednost širine pulza na 25 %. To širino spremenimo s tem ukazom: sConfigOC.Pulse = 25; 
Ukazi 1., 2. in 3. vrstice v user code begin 3 počnejo naslednje:
# 1.	Nastavi spremenljivko dutyCycle za dyuty cycle.
# 2.	Spremenljivki dutyCycle prišteje 10.
# 3.	Če spremenljivka dutyCycle preseže 90, jo ponastavi na 10.
# Komentar: Osciloskop prikaže PWM signal iz STM32F4 Discovery. Osciloskop je zelo preprosto nastaviti in tudi odčitati podatke iz njega je zelo preprosto. Potrebno je samo paziti, da pravilno nastavimo vse parametre v STM32CubeIDE, zato ker če jih ne nastavimo pravilno potem na izhodu ne dobimo pravega signala in ne moremo pravilno odčitati podatkov.
