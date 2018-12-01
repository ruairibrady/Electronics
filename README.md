# Electronics
## Excercise 5: RC Network Decay
This exercise examines the exponential decay of an [RC network](https://github.com/ruairibrady/Electronics/blob/master/1.%20RC%20network%20decay%20(5)/5_circuit.JPG) as a 2.5 V square wave is driven through it using three different methods. Firstly, an equation detailing the circuit’s theoretical decay is derived according to Kirchhoff’s Voltage Law. It is found that when the time equals the product of the resistor and capacitor used, a special point known as the circuit time constant is reached. Here, the voltage output of the system will have decayed by [63% its initial input](https://github.com/ruairibrady/Electronics/blob/master/1.%20RC%20network%20decay%20(5)/Theory/40.1_5_resistances.ipynb). For this RC network, a resistor and capacitor of strength 1.0 kΩ and 1 μF are used to provide a theoretical time constant value of 1 ms. A simulation of the circuit is then run using the SPICE based electronics design software TINA and a time constant value of [0.997 ± 0.001 ms](https://github.com/ruairibrady/Electronics/blob/master/1.%20RC%20network%20decay%20(5)/Simulation/5_simulation.jpg) is gotten. Along with this, the circuit was constructed on a breadboard to be physically analysed. A digital oscilloscope recorded an experimental time constant value of [1.00 ± 0.01 ms](https://github.com/ruairibrady/Electronics/blob/master/1.%20RC%20network%20decay%20(5)/Experimental/5_oscilloscope.png) for the system.
## Excercise 7: RC Amplitude and Phase
This exercise examines the Bode plots of the [RC network](https://github.com/ruairibrady/Electronics/blob/master/2.%20RC%20amplitude%20and%20phase%20(7)/7_circuit.JPG) discussed in exercise 5 previous. The gain and phase change is studied as a 2.5 V sinusoidal alternating wave is driven through the circuit at a range of different frequencies. Once again, the various outcomes are analysed using three different methods. Firstly, a set of equations detailing the circuit’s theoretical gain and phase change are derived. When the time equals the product of the resistor and capacitor used, the time constant is once again reached where the capacitor is 63% charged. The oscillating frequency \omega corresponds to the inverse of this time constant value. It is found that at this point, \omega, the amplitude of the transmitted signal has a gain of approximately -3.01 dB and a phase angle change of 45°. A simulation of the circuit is then run using the SPICE based electronics design software TINA and it is found that a [gain of -3.01 dB]((https://github.com/ruairibrady/Electronics/blob/master/2.%20RC%20amplitude%20and%20phase%20(7)/amplitude/Simulation/7_simulation_amplitude.jpg)) occurs at \omega = 9.980x10-4. It also found that a [phase change of 45°](https://github.com/ruairibrady/Electronics/blob/master/2.%20RC%20amplitude%20and%20phase%20(7)/phase/Simulation/7_simulation_phase.jpg) occurred at \omega = 1.000x10-4. Finally, the output voltage was recorded and compared to the input voltage for the circuit constructed in exercise 5 as the frequency varied. The data collected allowed for a set of experimental Bode plots to be created. It was found that a [gain of -3.01 dB](https://github.com/ruairibrady/Electronics/blob/master/2.%20RC%20amplitude%20and%20phase%20(7)/amplitude/Experimental/40.2_7_amplitude.ipynb) was gotten with a [phase change of 45.0°](https://github.com/ruairibrady/Electronics/blob/master/2.%20RC%20amplitude%20and%20phase%20(7)/phase/Experimental/40.3_7_phase.ipynb).
## Excercise 12A: Diode IV Curves
In this exercise the semiconducting device known as the diode is studied. In section 12A the device is used as a switch and the corresponding IV curves are examined for the 1N4148 diode using three different methods. The IV diode characteristic equation is defined and used to plot the [expected theoretical IV curve](https://github.com/ruairibrady/Electronics/blob/master/3.%20Diode%20IV%20(12A)/Theory/Diode%20Equation%20Plots/40.5_12A_IV_equation_plots.ipynb) for the device. Then, using TINA a [simulation](https://github.com/ruairibrady/Electronics/blob/master/3.%20Diode%20IV%20(12A)/Simulation/40.6_12A_simulated.ipynb) is run to obtain a similar IV plot. The circuit shown is then constructed on a breadboard. A voltmeter and ammeter were attached, and data was recorded for the voltage going across the diode and the current passing through it. The [experimental IV curve](https://github.com/ruairibrady/Electronics/blob/master/3.%20Diode%20IV%20(12A)/Experimental/40.7_12A_IV_experimental.ipynb) showed a plot which required a voltage of 0.80 V to breakdown the depletion barrier of the diode. Comparing this to the theoretical and simulated plots a value of 0.70 V was expected for the silicon based diode. This discrepancy between the experimental and theoretical/simulated value for depletion barrier breakdown voltage may be due to a manufacturing error in the device.
## Excercise 12B: Diode IV Curve (Capacitor)
In section 12B of the exercise the 1N4148 diode’s ability to functionality as a half wave rectifier is examined. The [circuit](https://github.com/ruairibrady/Electronics/blob/master/4.%20Diode%20IV%20capacitor%20(12B)/12B_circuit_2.JPG) shown is driven with a sinusoidal waveform of 500 Hz and amplitude 1.5 V. The [input is compared to the output](https://github.com/ruairibrady/Electronics/blob/master/4.%20Diode%20IV%20capacitor%20(12B)/Experimental/12B_3V_500Hz.png) across the resistor. The device blocks any waveform elements corresponding to a reverse bias setup with regards to the diode. This results in a direct voltage output of amplitude 0.70 V, this further aligns with the experimental depletion barrier breakdown voltage of 0.80 V recorded in section 12A. A [1 μF capacitor is then added](https://github.com/ruairibrady/Electronics/blob/master/4.%20Diode%20IV%20capacitor%20(12B)/12B_circuit_1.JPG) to the device to examine its ability to remove the altering current elements existing within the output waveform of the diode. The [ripple output voltage produced](https://github.com/ruairibrady/Electronics/blob/master/4.%20Diode%20IV%20capacitor%20(12B)/Experimental/12B_3V_500Hz_Capacitor.png) is analysed using a simulation (R = 470 Ω and Vin = 3 V) and experimentally (R = 1000 Ω and Vin = 1.5 V). The theoretical calculation expects a peak to peak amplitude of 0.64 V for the simulation and 0.15 V for the experimental circuit (figure 25 lower) to be produced. To compare, values of 0.15 V and 0.65 V were recorded for the two values respectively.
## Excercises 19, 20 and 21: Transistors
Throughout these exercises the transistor is studied, and its practical uses are explored. In [exercise 19](https://github.com/ruairibrady/Electronics/blob/master/5.%20Transistor%20amplification%20(19)/19_circuit.JPG) such [amplification properties](https://github.com/ruairibrady/Electronics/blob/master/5.%20Transistor%20amplification%20(19)/19_voltages.jpg) are analysed whilst in [exercise 20](https://github.com/ruairibrady/Electronics/blob/master/6.%20Transistor%20switch%20(20)/20_circuit.JPG) the device is used as a [functioning switch](https://github.com/ruairibrady/Electronics/blob/master/6.%20Transistor%20switch%20(20)/20_plot.jpg). Exercise 21 combines the [theory](https://github.com/ruairibrady/Electronics/blob/master/7.%20Light%20sensitive%20alarm%20(21)/40.8_21_resistances.ipynb) from the two previous exercises and a functioning [light dependent alarm](https://github.com/ruairibrady/Electronics/blob/master/7.%20Light%20sensitive%20alarm%20(21)/21_circuit_moon.JPG) is constructed experimentally.
## Excercise 25: Operational Amplifier Amplification
Exercise 25 examines the unique amplification properties of the operational amplifier. The [external resistors](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/Theory/40.9_25_resistor_calculator.ipynb) required to produce a gain of 20 dB are calculated using an equation derived from the voltage divider relationship. It is found that R2 must be 9 times greater than R1. 21 This device was then simulated using TINA and the [output of the non-inverting amplifier is compared to the input voltage](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/Simulation/No%20Capacitor/25_voltages_simulation.jpg). The design is then [constructed experimentally](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/25_circuit.JPG) using a resistor ratio of 10 to produce a gain of 20.83 dB. The frequency response curves for the circuit gain is then [simulated](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/Simulation/No%20Capacitor/25_amplitude_simulation.jpg) and analysed [experimentally](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/Experimental/No%20Capacitor/40.11_25_amplitude.ipynb). A 1 μF capacitor is then added across the resistor R2 to examine its effect on the bandwidth. The voltage output is examined both [theoretically](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/Simulation/Capacitor/25_amplitude_capacitor_simulation.jpg), and [experimentally](https://github.com/ruairibrady/Electronics/blob/master/8.%20Op-amp%20amplification%20(25)/Experimental/Capcitor/40.10_25_amplitude_cap.ipynb) it is found that the capacitor causes the gain to decrease at much lower frequencies.
## Excercise 27: Inverting Amplifier Digital to Analogue Converter
In this exercise the [summing amplifier](https://github.com/ruairibrady/Electronics/blob/master/9.%20Op-amp%20DAC%20(27)/27_circuit.JPG) is used to produce a 4-bit digital to analogue converter (DAC). Binary weighted resistors are used in tangent with the inverting amplifier to create a DAC. The number of switches and resistor components used in the device directly corresponds to the number of bits available for processing. For correct functioning of the DAC each of the resistors must be functioning at the correct ratio (1:2:4:8) and at equal temperature. The expected [voltage output](https://github.com/ruairibrady/Electronics/blob/master/9.%20Op-amp%20DAC%20(27)/40.12_27_voltages.ipynb) was calculated.
