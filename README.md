# BlinkLED_Blue_Pill_Timer

Ce programme fonctionne sur une carte de devellopement appelé Blue Pill. Elle utilise un MCU STM32F103C8

## Fonctionnement

La fréquence interne du MCU est de 8 Mhz tout comme le timer1. LE timer1 est configuré pour lever une interruption toutes les secondes,  le prescaler est réglé sur 8000 et le couter période sur 1000.

FreqIT = FreqTIMER / Prescaler / CouterPeriode = 1Hz

La routine d'intérruption va inverser l'état de la LED.
