# DC_simulink_project

# How to reproduce the scatter plot for one of the schemes:
- 1- Open Matlab 2016 (won't work on matlab 2017).
- 2- Run the ```simulink``` command from the command window.
- 3- Open the file (.slk or .mdl), then hit run button.
---
# How to rebuild a scheme:
- 1- Open Matlab 2016 (won't work on matlab 2017).
- 2- Run the ```simulink``` command from the command window.
- 3- Open ```library browser``` from view.
- 4- Drag and drop the components and connect them.
---
# How to generate ber diagram:
- 1- Run the ```bertool``` command from the command window.
- 2- Select Monte carlo.
- 3- Browse and load the model, set parameters then run.
---
# **Binary Phase-Shift Keying Modulation (BPSK)**
## Explanation:
Phase Shift Keying (PSK) is the digital modulation technique in which the phase of the carrier signal is changed by varying the sine and cosine inputs at a particular time. PSK has two types first one is BPSK. BPSK is a two phase modulation scheme, where the 0’s and 1’s in a binary message are represented by two different phase states in the carrier signal: θ=0∘ for binary 1 and θ=180∘ for binary 0.

So in the scheme we start with passing the signal through BPSK modulator and after the AWGN channel(simulating real channel) we receive the signal in BPSK demodulator. Then we calculate the bit error rate.  

## BPSK without Raised Cosine Filter
### Simulink Model Diagram:
![Model](/BPSK/bpsk_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot(BeforeNoise)](/BPSK/bpsk_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/BPSK/bpsk_ber.PNG)

## BPSK with Raised Cosine Filter
### Simulink Model Diagram:
![Model](/BPSK_rc/bpsk_rc_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot(BeforeNoise)](/BPSK_rc/bpsk_rc_scatter_plot.PNG)
---
# **Quadrature Phase Shift Keying (QPSK)**
## Explanation:
Phase Shift Keying (PSK) is the digital modulation technique in which the phase of the carrier signal is changed by varying the sine and cosine inputs at a particular time. PSK has two types second one is QPSK. QPSK is phase shift keying technique, in which the sine wave carrier takes four phase reversals such as 0°, 90°, 180°, and 270°. Can be done by eight or sixteen values also.

So in the scheme we start with passing the signal through QPSK modulator and after the AWGN channel(simulating real channel) we receive the signal in QPSK demodulator. Then we calculate the bit error rate.  

## QPSK without Raised Cosine Filter
### Simulink Model Diagram:
![Model](/QPSK/qpsk_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/QPSK/qpsk_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/QPSK/qpsk_ber.PNG)

## QPSK with Raised Cosine Filter
### Simulink Model Diagram:
![Model](/QPSK_rc/qpsk_rc_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/QPSK_rc/qpsk_rc_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/QPSK_rc/qpsk_rc_ber.PNG)

---
# **Quadrature amplitude modulation (QAM)**
## Explanation:
QAM is a signal in which two carriers shifted in phase by 90 degrees (sine and cosine) are modulated and combined. As a result of their 90° phase difference they are in quadrature and this gives rise to the name. QAM provides some significant benefits for data transmission. As QAM16 and QAM64. higher data rates can be achieved, but at the cost of the noise margin.

So in the scheme we start with passing the signal through QAM modulator and after the AWGN channel(simulating real channel) we receive the signal in QAM demodulator. Then we calculate the bit error rate.  

## QAM_16 without Raised Cosine Filter
### Simulink Model Diagram:
![Model](/QAM16/qam16_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/QAM16/qam16_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/QAM16/qam16_ber.PNG)

## QAM_16 with Raised Cosine Filter
### Simulink Model Diagram:
![Model](/QAM16_rc/qam16_rc_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/QAM16_rc/qam16_rc_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/QAM16_rc/qam16_rc_ber.PNG)

## QAM_64 without Raised Cosine Filter
### Simulink Model Diagram:
![Model](/QAM64/qam64_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/QAM64/qam64_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/QAM64/qam64_ber.PNG)

## QAM_64 with Raised Cosine Filter
### Simulink Model Diagram:
![Model](/QAM64_rc/qam64_rc_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/QAM64_rc/qam64_rc_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/QAM64_rc/qam64_rc_ber.PNG)


# **Frequency Shift Keying (FSK)**
## Explanation:
Phase Shift Keying (PSK) is the digital modulation technique in which the phase of the carrier signal is changed by varying the sine and cosine inputs at a particular time. PSK has two types second one is QPSK. QPSK is phase shift keying technique, in which the sine wave carrier takes four phase reversals such as 0°, 90°, 180°, and 270°. Can be done by eight or sixteen values also.

So in the scheme we start with passing the signal through FSK modulator and after the AWGN channel(simulating real channel) we receive the signal in FSK demodulator. Then we calculate the bit error rate.  

## FSK without Raised Cosine Filter
### Simulink Model Diagram:
![Model](/FSK/fsk_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/FSK/fsk_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/FSK/fsk_ber.PNG)

## FSK with Raised Cosine Filter
### Simulink Model Diagram:
![Model](/FSK_rc/fsk_rc_scheme.PNG)
### Scatter Plot (Before and after the noise)
![ScatterPlot](/FSK_rc/fsk_rc_scatter_plot.PNG)
### BER Performance Plot
![BER-Plot](/FSK_rc/fsk_rc_ber.PNG)

