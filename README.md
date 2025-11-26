# DSB--SC-MODULATION-AND-DEMODULATION-USING-PYTHON

__AIM__:

To generate a Double Sideband Suppressed Carrier (DSB-SC) signal in Python (Google Colab), transmit it (optionally add noise), and recover the message using coherent (synchronous) demodulation with a low-pass filter. Observe time and frequency domain waveforms and measure demodulation performance

__APPARATUS REQUIRED__:

Google Colab (or any Python environment)

Python libraries: numpy, matplotlib, scipy (scipy.signal)

__Theory__:

DSB-SC signal: s(t) = m(t) · cos(2πf_c t)
Coherent demodulation: multiply received s(t) by a synchronized carrier cos(2πf_c t) then low-pass filter (LPF) to remove double-frequency components:

r(t) = s(t)·cos(2πf_c t) = m(t)·cos²(2πf_c t) = 0.5 m(t) + 0.5 m(t)·cos(4πf_c t)
LPF extracts 0.5·m(t) → scale by 2 to recover m(t).

__Procedure__:

1) Import libraries and set parameters
2) Define message and carrier signals
3) Generate DSB-SC signal (modulation)
4) View spectra (FFT) of message and DSB-SC
5) (Optional) Add noise
6) Coherent demodulation (multiply by synchronized carrier)
7) Low-pass filter to recover message

   __Tabulation__:
![WhatsApp Image 2025-11-26 at 22 43 52_8d67678a](https://github.com/user-attachments/assets/25899e0e-92ee-40ec-923a-a35c0708e3fd)

![WhatsApp Image 2025-11-26 at 22 45 27_fb81de0a](https://github.com/user-attachments/assets/cc3450c9-9009-4cde-9b37-6f67ab4985b5)



   __Output__:
<img width="989" height="590" alt="image" src="https://github.com/user-attachments/assets/4e00e5b8-9832-4091-8037-ed6221b3206b" />

   __Result__:
![WhatsApp Image 2025-11-23 at 15 12 21_d521a2d3](https://github.com/user-attachments/assets/89574433-900b-49e4-84df-544f41a71803)
