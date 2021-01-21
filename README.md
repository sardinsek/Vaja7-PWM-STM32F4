# Vaja7-PWM-STM32F4
Prvi kanal sva aktivirala kot PWM Generation CH1. Omogočila sva pin PE9. Poleg njega pa se izpiše oznaka TIM1_CH1.
Vrednost Perscaler sva nastavila na 16.
Parameter Counter Period sva nastavila na 100 in s tem še dodatno znižala takt časovnika. Takt sedaj znaša 10 kHz.
V PWM Generation Chanel sva nastavila Pulse (16 bits value) na 50. Ta parameter pomeni, da delovni cikel deluje na 50 % svoje zmogljivosti.
