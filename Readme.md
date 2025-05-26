# Stretched hollow-core fiber pulse compressor
## A. Weber, H. Hampel, A. Grossek, M. Schultze, M. Ossiander

The compressor setup described was constructed as part of my bachelor's thesis at the Institute for Experimental Physics (IEP) of the TU Graz. The setup is similar to one constructed by Z. Pi, H. Y. Kim, and E. Goulielmakis and a pulse compressor that already perviously was constructed at the IEP by Hana Hampel.
>Z. Pi, H. Y. Kim, and E. Goulielmakis, "Petahertz-scale spectral broadening and few-cycle compression of Yb:KGW laser pulses in a pressurized, gas-filled hollow-core fiber," Opt. Lett. 47, 5865-5868 (2022)
 
It uses a high-pressure Ne-filled stretched hollow-core fused silica fiber to broaden the spectrum of a Yb:KGW Pharos laser (Light Conversion, center wavelength: 1030 nm, pulse duration: 150 fs, repetition rate: 6 kHz, average power: 6 W) via self-phase modulation. The Fourier limited pulse duration suggested by the output spectrum is 9 fs (intensity FWHM).

<p align="center">
  <img src="https://github.com/user-attachments/assets/41ae047a-e041-4681-b4ed-95bda4435030" width="400">
  <br>
  <em>On the left hand side of this image, the vessel housing of the other compressor is visible.
Alongside to it is the stretched hollow-core fiber compressor, contained within a significantly
smaller vessel.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/d56808f9-6d11-428b-9e61-e7613f694baa" width="600">
  <br>
  <em>Measured output spectra and transmitted power vs. neon pressure. The input power was ~5.5 W.</em>
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/86961dcd-ef2a-4f07-a293-535d65e2c267" width="600">
  <br>
  <em>Fourier transform limited pulse duration.</em>
</p>

# Pressure Vessel Considerations
The pressure vessel can withstand pressures up to 25 bar (with a safety factor of 2); the critical parts are the windows.
We use 2 mm-thick BK7 windows with a free aperture of 12 mm. Pressures exceeding 25 bar require a calculation to ensure the windows will withstand the pressure. Suitable formulas are, e.g., found here https://www.crystran.com/media/wysiwyg/Datasheets/design-of-pressure-windows_1.pdf.
 
An appropriate distance between the entrance and exit window and the entrance and exit of the fiber (focal point) prevents the laser from destroying the windows. For our laser setup, 45 cm work. This depends on the laser pulse parameters and focusing optics used.

In our first approach, we use Brewster angle windows to maximize transmission. Their handling is slightly harder than that of a window oriented perpendicular to the laser beam, due to an offset the beam experiences as it propagates through the glass. Both designs are functional; however, perpendicular windows with anti-reflective coatings have proven to be more practical and easier to implement. Owing to the broad spectral width, Brewster angle windows are still employed for the vessel's exit window to minimize reflection losses.

Additionally, we constructed slightly larger housings to accommodate aluminum extrusions with a greater diameter, as thinner profiles often exhibit deviations from straightness.

<p align="center">
  <img src="https://github.com/user-attachments/assets/edd0fb60-0807-45a9-a198-e88b30f126b0" width="900">
  <br>
  <em>3D model of the pressure vessel.</em>
</p>


# Fiber Considerations
To improve coupling efficiency, it is important to match the beam waist radius (w) to the bore radius (a) of the fiber. The ideal beam waist can be calculated using the following formula: w ≈ 0.64 * a. 
>T. Nagy, P. Simon and L. Veisz, "High-energy few-cycle pulses: post-compression techniques", Advances in Physics: X, 6(1), 
https://doi.org/10.1080/23746149.2020.1845795, (2020)

The utilized fiber was a stretched molex TSP250794 (bore diameter: 250 μm, outer diameter: 794 μm, length: 1.1 m), which was mounted in an aluminum profile.

# Repository Structure
This repository contains equivalent drawings of the compressor in .stp and in .itp format (used by Autodesk Inventor). Each folder contains a file named "full_vessel," which contains the assembled structure. 

For more information, have a look at my bachelors thesis and feel free to ask questions. 

# License
The contents of the folders components_cc_stp and components_cc_itp are licensed under the terms of the CC BY 4.0 Creative Commons Attribution 4.0 International (full license: https://creativecommons.org/licenses/by/4.0/ ).

This open licensing does not apply to the CF components in the folders componetns_PfeifferVacuum_stp and components_PfeifferVacuum_itp which were provided by Pfeiffer Vacuum as .stp-models at https://vacuum-shop.com/shop/de_DE/ . We thank Pfeiffer Vacuum for allowing us to use their models.
