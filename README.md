# Low poly water for Unity written with shaders to simulate the water using the linear wave equations and the shallow water equations. #
To come:  
- [x] implementing Shallow Water Equations instead of current version  
- [x] improving shading  
- [ ] add shadows    
- [ ] allow arbitrary large water mesh (currently clamped at 254 x 254)  
- [ ] apply shader to any mesh  
- [x] interactive water (additional script required)
          
## Preview ##
![Alt Text](https://github.com/sc2insane/Lowpoly-water-for-Unity/raw/dev/Gifs/lowpolywater.gif)

Currently Possible:  
          * add random noise to vertices positions  
          * change behaviour of water (damping, maxHeight, maxVelocity, initialRandomVelocity)  
          * access heightfield to generate waves, etc.  
          * adjust size of generated mesh  
                
Heightfield.cs accesses the sun position, forward vector and color for computing the specular highlights/reflections. Make sure to set the compute buffer and main camera in the script.
