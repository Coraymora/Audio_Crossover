# Audio_Crossover
This is a straightforward active audio-crossover circuit utilizing Linkwitz-Riley filters.

An audio crossover circuit splits an incoming audio signal into frequency bands that can be passed to seperate speakers. The simplest type of crossover would utilize only a few passive components for filtering, but replacing these with active filters (usign audio op-amps) allows us to amplify each channel individually, which is the goal of this project.

![image](https://github.com/Coraymora/Audio_Crossover/assets/68129788/ed9a8c12-57a7-4863-935a-93aec6808ad0)

![image](https://github.com/Coraymora/Audio_Crossover/assets/68129788/39c8de2b-ace1-4de0-a910-d8d774a3d9c2)

  Fig 1. Photographs of breadboard prototype

As can be seen in the photographs above, we use a pair of 5W-8ohm speakers, two potentiometers, and an aux cable to test the system. Note that we deviated from the original design by replacing the BJT amplifier stage with op-amps.

![image](https://github.com/Coraymora/Audio_Crossover/assets/68129788/d03e5461-e6e9-43e9-9a70-1500d88fbee2)
  
  Fig 2. LTSpice schematic

The Linkwitz-Riley design is often used for filtering in crossover circuits, because it produces a flat response at the crossover point (where the response from the high-pass filter and low-pass filter overlap), which is desirable in audio applications.

![image](https://github.com/Coraymora/Audio_Crossover/assets/68129788/db035452-d73e-4a21-962c-c72049ef7cea)
  
  Fig 3. LTSpice simulation of high-pass (green) and low-pass (blue) filters

![image](https://github.com/Coraymora/Audio_Crossover/assets/68129788/cc20f2ba-b40a-432c-b446-4515728e8f3d)

![image](https://github.com/Coraymora/Audio_Crossover/assets/68129788/88796b59-2e73-41d8-9e26-d724e14e73db)

  Fig 4. Bode plots of high-pass and low-pass filters measured with NI MyDAQ
