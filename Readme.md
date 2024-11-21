# Stretched hollow-core fiber pulse compressor
## A. Weber, H. Hampel, A. Grossek, M. Schultze, M. Ossiander

The compressor setup described was constructed as part of my bachelor's thesis at the Institute for Experimental Physics (IEP) of the TU Graz. The setup is similar to one constructed by Z. Pi, H. Y. Kim, and E. Goulielmakis and a pulse compressor that already perviously was constructed at the IEP by Hana Hampel.
>Z. Pi, H. Y. Kim, and E. Goulielmakis, "Petahertz-scale spectral broadening and few-cycle compression of Yb:KGW laser pulses in a pressurized, gas-filled hollow-core fiber," Opt. Lett. 47, 5865-5868 (2022)
 
It uses a high-pressure Ne-filled stretched hollow-core fused silica fiber to broaden the spectrum of a Yb:KGW Pharos laser (Light Conversion, center wavelength: 1030 nm, pulse duration: 150 fs, repetition rate: 6 kHz, average power: 6 W) via self-phase modulation. The Fourier limited pulse duration suggested by the output spectrum is 9 fs (intensity FWHM).

BILD VOM COMPRESSOR

<p align="center">
  <img src="https://github.com/user-attachments/assets/d56808f9-6d11-428b-9e61-e7613f694baa" width="600">
  <br>
  <em>Measured output spectra and transmitted power vs. neon pressure. The input power was ~5.5 W.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/8cb8a2ef-0e3d-4c3d-bc1a-aeede7eeac41" width="600">
  <br>
  <em>Fourier transform limited pulse duration.</em>
</p>

# Pressure Vessel Considerations
The pressure vessel can withstand pressures up to 25 bar (with a safety factor of 2); the critical parts are the windows.
We use 2 mm-thick BK7 windows with a free aperture of 12 mm. Pressures exceeding 25 bar require a calculation to ensure the windows will withstand the pressure. Suitable formulas are, e.g., found here https://www.crystran.com/media/wysiwyg/Datasheets/design-of-pressure-windows_1.pdf.
 
An appropriate distance between the entrance and exit window and the entrance and exit of the fiber (focal point) prevents the laser from destroying the windows. For our laser setup, 45 cm work. This depends on the laser pulse parameters and focusing optics used.

In our first approach, we use Brewster angle windows to maximize transmission. Their handling is slightly harder than that of a window oriented perpendicular to the laser beam, due to an offset the beam experiences as it propagates through the glass. We will update the plans as we learn what works best.

# Fiber Considerations
To improve coupling efficiency, it is important to match the beam waist radius (w) to the bore radius (a) of the fiber. The ideal beam waist can be calculated using the following formula: w ≈ 0.64 * a 
>T. Nagy, P. Simon and L. Veisz, "High-energy few-cycle pulses: post-compression techniques", Advances in Physics: X, 6(1), 
https://doi.org/10.1080/23746149.2020.1845795, (2020)

# Repository Structure
This repository contains equivalent drawings of the compressor in .stp and in .itp format (used by Autodesk Inventor). Each folder contains a file named "full_vessel," which contains the assembled structure. 

For more information, have a look at my bachelors thesis and feel free to ask questions. 

# License
The contents of the folders ____ are licensed under the terms of the CC BY 4.0 Creative Commons Attribution 4.0 International (full license: https://creativecommons.org/licenses/by/4.0/ ).

This open licensing does not apply to the CF components in the folders ____ which were provided by Pfeiffer Vacuum as .stp-models at https://vacuum-shop.com/shop/de_DE/ . We thank Pfeiffer Vacuum for allowing us to use their models.
