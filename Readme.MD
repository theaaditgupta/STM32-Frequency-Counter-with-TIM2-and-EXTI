Coordinated weddings, conferences, and private events from planning through execution, ensuring seamless delivery and high client satisfaction.

Served as the primary client liaison, translating client requirements into actionable event plans and resolving concerns promptly to maintain service quality.

Organized room layouts, décor, audiovisual requirements, and vendor logistics, ensuring smooth event flow and on-time setups.

Led and supported banquet and culinary teams during live events, aligning staffing and resources to deliver consistent, high-quality service.

Managed event timelines, last-minute changes, and on-site problem solving, minimizing disruptions and ensuring successful outcomes.

Ensured full compliance with hotel standards, health, and safety regulaSTM32 Signal Frequency Measurement

This project implements a signal frequency and period measurement system on an STM32F051 microcontroller using external interrupts and Timer 2.

The program detects a signal on GPIO pin PA2, measures the time between rising edges using a hardware timer, and calculates the signal frequency and period.

Features

Configures the system clock to 48 MHz

Uses EXTI interrupt on PA2 to detect rising edges

Uses TIM2 hardware timer to measure elapsed time

Calculates:

Signal frequency (Hz)

Signal period (microseconds)

Outputs results through trace debugging

How It Works

External signal arrives at PA2

First rising edge:

Timer starts counting

Second rising edge:

Timer stops

Counter value is read

Period is calculated:

Period=Timer CountSystem Clock
Period=
System Clock
Timer Count
	​


Frequency is calculated:

Frequency=1Period
Frequency=
Period
1
	​


Results are printed through the debug trace.

Key Components

GPIOA PA2 – Input signal

EXTI2 interrupt – Detects rising edge

TIM2 – Measures time between edges

NVIC – Handles interrupt priorities

System Clock – Configured to 48 MHz

Example Output
Signal Frequency: 1000 Hz
Signal Period: 1000 us

Technologies

Embedded C

STM32F0 Microcontroller

ARM CMSIS

Hardware Timers

Interrupt Handling

Course

ECE 355 – Microprocessor-Based Systems
University of Victoria

Author

Aadit Gupta
Electrical & Computer Engineering