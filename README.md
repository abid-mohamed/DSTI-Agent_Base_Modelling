# ABM for Underwater optical wireless communication in a water tank

![image-Underwater-optical-wireless-communication-in-a-water-tank](https://www.comses.net/media/images/sharedlibrary23ce38af-ae87-47bf-b9e3-2523a54.max-900x600.png)

This model simulates the propagation of photons in a water tank. A source of light emits an impulse of photons with equal energy represented by yellow dots. These photons are then scattered by water particles before possibly reaching the photo-detector represented by a gray line. Different types of water are considered. For each one of them we calculate the total received energy.

The water tank is represented by a blue rectangle with fixed dimensions. It’s exposed to the air interface and has totally absorbent barriers. Four types of water are supported. Each one is characterized by its absorption and scattering coefficients. <br />
At the source, the photons are generated uniformly with a random direction within the beamwidth. Each photon travels a random distance drawn from a distribution depending on the water characteristics before encountering a water particle. <br />
Based on the updated position of the photon, three situations may occur: <br />
<br />
    - The photon hits the barrier of the tank on its trajectory. In this case it’s considered as lost since the barriers are assumed totally absorbent. <br />
<br />
    - The photon hits the top of the water. Depending on the incident angle, two cases occur: <br />
	    * If the incident angle is greater than the critical angle, the photon is reflected without loss of energy. <br />
	    * If the incident angle is smaller than the critical angle, the photon is reflected with a loss of energy depending on the Fresnel coefficient. <br />
<br />
	- The photon hits a particle. In this case it undergoes a loss of energy depending on the water characteristics and then gets deviated by a random angle following the Henyey–Greenstein Model. <br />
<br />    	
The above process is repeated until either the photon is lost or it reaches the photo-detector. <br />

Mohamed ABID (2022, May 29). “ABM for Underwater optical wireless communication in a water tank” (Version 1.0.0). CoMSES Computational Model Library. Retrieved from: https://www.comses.net/codebases/23ce38af-ae87-47bf-b9e3-2523a54fe1a1/releases/1.0.0/