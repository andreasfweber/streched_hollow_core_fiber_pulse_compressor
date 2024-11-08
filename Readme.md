# Stretched-hollow-core-fiber-pulse-compressor
The compressor setup described was constructed as part of my bachelor's thesis at the Institute for Experimental Physics (IEP) of the TU Graz. I was supervised by Marcus Ossiander. The setup is similar to those constructed by Z. Pi, H. Y. Kim, and E. Goulielmakis and a pulse compressor constructed at the IEP by Hana Hampel.
>Z. Pi, H. Y. Kim, and E. Goulielmakis, "Petahertz-scale spectral broadening and few-cycle compression of Yb:KGW laser pulses in a pressurized, 
gas-filled hollow-core fiber," Opt. Lett. 47, 5865-5868 (2022)
 
It uses a high-pressure Ne-filled stretched hollow-core silica fiber to broaden the spectrum of a Yb:KGW laser from Pharos (center wavelength: 1030 nm, pulse duration 150 fs, 6 W) by self-phase modulation. We checked the Fourier transform limit pulse duration by inverse Fourier transforming the wavelength-dependent intensity data from the frequency domain to the time domain to obtain the FWHM of the intensity, which is the most common definition of pulse duration. The time-domain FWHM of the intensity was 8.91 fs.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d56808f9-6d11-428b-9e61-e7613f694baa" width="600">
  <br>
  <em>Measured spectra: The corresponding pressure in the vessel and the power measured at the exit window. The input power was around 5.47 W</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/8cb8a2ef-0e3d-4c3d-bc1a-aeede7eeac41" width="600">
  <br>
  <em>Fourier transform limit pulse duration</em>
</p>
hello
# Considerations
The pressure vessel itself is designed to withstand pressures up to 25 bar. While the CF components could withstand much higher pressures, the critical part is the windows.
I used BK7 with a thickness of 2 mm and a diameter of 12 mm. If you want to use pressures ecceeding 25 bar you could do a quick calculation to make sure that the windows will withstand the pressure. Suitable formulas can be found online, for example at https://www.crystran.com/media/wysiwyg/Datasheets/design-of-pressure-windows_1.pdf.
 
Also consider an appropriate distance between the focal point at the beginning of the fiber and the entrance window, depending on the laser and focusing optics you are using, to prevent the laser from destroying the window. For this setup, 45 cm should work.
 
The exit window is oriented at the Brewster angle corresponding to the refractive index of the glass and the center wavelength of the laser. In our first approach, we also used a Brewster entrance window - which is probably even slightly worse than a window oriented perpendicular to the laser beam, due to the offset the beam gets as it propagates through the glass. I'll update the plans as I learn what works best.

To improve your coupling efficiency, it is important to match the beam waist radius w to the bore radius a of the fiber. The ideal beam waist can be calculated using the following formula: w ≈ 0.64 * a 
>T. Nagy, P. Simon and L. Veisz, "High-energy few-cycle pulses: post-compression techniques", Advances in Physics: X, 6(1), 
https://doi.org/10.1080/23746149.2020.1845795, (2020)

You can find most of the parts I used in my plan as 3D models suitable for the CAD program of your choice at https://vacuum-shop.com/shop/de_DE/.

For more information, have a look at my bachelors thesis and feel free to ask questions. 




