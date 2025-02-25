<h1 align=center>Coherent Light Simulation of Speckle Interference Patterns in Optical Metrology</h1>

<h5 align=center>Spatial Light Modulator Based Propagation of Partially Coherent Speckle Fields in a 4f setup<h5>


<h6 align="center"><a href="https://schulze-paul.github.io">Paul Schulze</a></h6>

<h6 align=center>University of Bremen</h6>
	
<p align=center>
	<a href="https://raw.githubusercontent.com/schulze-paul/BIAS-SPICE/master/BachelorThesis.pdf">Thesis</a> • <a href="https://raw.githubusercontent.com/schulze-paul/BIAS-SPICE/master/BA_Paul_Schulze_Presentation.pdf">Presentation</a>


<h1 align=center >Abstract</h1>
Contrast measurements of interference patterns emerging from the surface can be used to
evaluate the three dimensional shape of an object. Traditionally, moving the focal plane through
the object involves a mechanical movement in the imaging system. In my thesis, I show that a
spatial light modulator (SLM) utilizing the transfer function of propagation can move the focal
plane with no reduction in image quality and without the need for any mechanical movement. The
SLM is integrated in the Fourier plane of a 4f imaging system. The speckle patterns (interference
patterns) play a central role in the evaluation process of the three dimensional measurement.
I report my findings from a simulation, which relate the size of the speckle to the wavelength
of light used as illumination, the size of the Fourier aperture and the focal length of the utilized
lenses in the 4f setup. A method for speckle size detection is presented. For partially coherent
light, a predictable area of high contrast forms around the objects’ surface, with the rest of
the wave field being of lower contrast. The simulated results are supported by experimental
evidence. I experimentally demonstrate a visible difference in contrast and image sharpness for
microscopic surface features of different height. This paves the road for the development of a
fully functional measuring method that is precise, fast, robust against vibrations and exhibits an
extended depth of focus.

<h1 align=center >Simulation Results</h1>

<h3 align=center >Amplitude and Phase of Simulated Speckle</h3>
	
<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Specke_amp_phase.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="600"/>

</div>

<b>Figure 1. Amplitude and phase of numerically simulated coherent speckle wavefield in the sensor plane.</b>  
The amplitude consists of the characteristic speckle pattern. The phase distribution shows phase singularities (e.g. red arrow) and phase jumps (e.g. yellow arrow). I generated the wavefield with 128 scattering points on a square surface of size 5.42 mm × 5.42 mm,
10 mm from the input plane, illuminated with a wavelength of λ = 530 nm. The 4f setup
consists of two f = 100 mm lenses and a Fourier aperture of diameter ρ = 0.25 mm. The
sampled area shown is 512 × 512 pixels with a pixel pitch of ∆x = 5.2 µm. 

<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Specke_cross.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="300"/>

</div>	
<b>Figure 2. Cross section of the amplitude from the generated speckle field.</b>
I captured the intensities at different z by varying the transfer function Hz in the Fourier domain from z = -500 mm
to z = 500 mm. I generated the wavefield with the same parameters as Figure 3. The
sampled area shown is 1024 × 1024 pixels.

	
<h3 align=center >Intensity Histogram of Simulated Speckle</h3>
	
<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Intensity_Hist.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="300"/>

</div>

<b>Figure 3. Normalized intensity histogram of the calculated coherent speckle pattern.</b>  
An exponential function
f(I/¯I) = a/¯I exp(b · I/¯I) (blue line)
is fitted to the data (black dots). The
parameters a ≈ 1.01 and b ≈ −1.02
were determined. Both are very close
to the expected values a = 1 and b = -1.
The position of the data point at I/¯I = 0
is an artifact of the histogram calculation
algorithm. The data point is excluded
from the fit calculation.
	
	
<h3 align=center >Size of Simulated Speckle</h3>
	
<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Speckle_Size.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="600"/>

</div>

<b>Figure 4. Speckle size dependence on wavelength, aperture diameter and focal length in the
4f setup. </b>  
<b>a</b>, Amplitude distributions of speckle fields with different speckle sizes. <b>b</b>, <b>c</b>, <b>d</b>,
Speckle size ∆s plotted over the wavelength of light λ, the reciprocal of aperture diameter
1/ρ and focal length f, respectively. Linear curves were fitted against the data. Error bars
indicate 95% confidence intervals. Linear relationships can be observed in all three cases.
from the fit calculation.
	

	
<h3 align=center >Contrast in Simulated Partially Coherent Speckle
</h3>
	
<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Speckle_Contrast.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="600"/>

</div>

<b>Figure 5. Numerically calculated amplitude distributions of a partially coherent wavefield at
different propagation distances. </b>  
I placed the objects’ surface at z0 = 10 mm and scanned
through the incoherent wavefield by changing the transfer function Hz on the SLM accordingly.
The contrast changes with the distance to the objects’ surface. I calculated the amplitude
distributions from 1024 scattering points on a square surface of 5.42 mm × 5.42 mm, 10 mm
from the input plane, illuminated with monochromatic light of wavelength λ = 530 nm. The
wavefield was processed through a 4f optical filter with f = 150 mm and an aperture diameter
of ρ = 1 mm. The sampled areas shown are 256 × 256 pixels with a pixel pitch of ∆x ≈ 10 um.

	
<h3 align=center >Cross Section of Simulated Partially Coherent Speckle</h3>
	
<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Speckle_cross_section_figure.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="600"/>

</div>

<b>Figure 6. Cross section and contrast values of the simulated incoherent amplitude distributions near the objects’ surface.</b>  
<b>a</b>, Cross section of the wavefields’ amplitude. The amplitude slices at different z were calculated by varying the transfer function in the Fourier domain
from z = 9 mm to z = 11 mm. The area of high contrast surrounding the objects’ surface is
clearly identifiable. <b>b</b>, Contrast of the partially coherent interference pattern. zmax ≈ 1.2 mm
denotes the area where the contrast of the recorded intensity distribution is high.
	
<h2 align=center>Experimental Results</h2>
	

<h3 align=center >Size of Speckle in the Experiment</h3>
	
<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Aperture_Diameter.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="800"/>
</div>

<b>Figure 7. Influence of the aperture diameter in the Fourier plane on the intensity distribution in
the experiment.</b>  
The speckle become smaller as the aperture opens up. I illuminate the
object with a Helium-Neon-Laser (λ = 633 nm) that is coupled over a S = 200 µm optical
fiber in a collimator of effective focal length R = 18 mm. The lenses in the 4f setup were of
focal length f = 100 mm. The images captured are 512 × 512 pixels and 1.8 mm × 1.8 mm.
Circles indicating aperture size not to scale

	
<h3 align=center >SLM Propagation in the Experiment</h3>

<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Moving_Focal_Plane.PNG?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="800"/>
</div>

<b>Figure 8. Moving the focal plane via SLM.</b> 
<b>a</b>, Sharp image of the object in the input plane of the
4f setup with no SLM modulation. <b>b</b>, Blurred image of the object at distance z0 ≈ 10 mm from
the input plane with no SLM modulation. <b>c</b>, Sharp image of the object at distance z0 ≈ 10 mm
from the imaging plane with the SLM shifting the focal plane to z = 10 mm. The reduction of
brightness on the left side is owed to the fact that the light source is further away from the
object compared to image a.

	
<h3 align=center>Contrast Difference for Surface Features Under Partially Coherent Illumination in the Experiment</h3>

<div align="center">
	<img src="https://github.com/schulze-paul/BIAS-SPICE/blob/master/Figures/Contrast_difference.png?raw=true" alt="Simulation Results" title="Simulation Results" 
	width="700"/>
</div>

<b>Figure 9. Sharpness difference between steps in the surface at partially coherent illumination.</b> 
Numbers in white referring to step number. Red arrows indicating
area in focus, yellow arrows indicating area out of focus. The combined height of steps 4-8
adds up to 35 µm. <b>a</b>, Intensity distribution captured without SLM modulation. <b>b</b>, A transfer
function Hz for z = 3 mm is written on the SLM. This results in a shift of the focal plane
closer to the outermost ring. The parameters of the setup were set to: fiber opening diameter
S = 1.4 mm, effective collimator focal length R = 6 mm, wavelength of light λ = 530 nm, 4f
focal length f = 100 mm and aperture diameter ρ ≈ 6 mm

<h1 align=center>Conclusion</h1>
In the course of this work I investigated several aspects of a 4f setup with a spatial light modulator
in the Fourier plane. The spatial light modulator was instructed to display a phase shifting transfer
function of propagation. I studied the effect of the wavelength of light, the opening diameter of
the light source, the distance of the light source, as well as the focal length and the size of the
Fourier aperture. For coherent illumination, the size of the Speckle is affected (Figure 4, 7).
For partially coherent illumination, the area, where high contrast interference occurs, is affected
as well (Figure 6, 8).
This was examined both in a numerical simulation that I based off of Fourier optics, and in the
experimental system itself, which I set up and took into operation. In order to
address the spatial light modulator, I wrote a program that would detect and compensate misalignment between the optical axes and display the appropriate transfer function of propagation
onto the device.
