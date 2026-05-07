# Quiz8_9103
This repository contains initial ideation for the final project for the course 9103

## Part 1: Imaging Technique

! [An image of the moodboard](Assets/jsconfig.png)
_Fig 1: Ideation board denoting elements that can be implemented_

Spider-Man: Across the Spiderverse (2023) is an animated film that uses various techniques derieved from comic and traditional art style which is then translated into a digital animated format through noise. At the core of this language is halftone textures that breathe across the surface, geometric structures (the multiverse portal) that rotate with seemingly random offests and particle clusters that disperse organically through space. The movie has an interesting take on portraying interactive elements which can be applied to the elements in the final project using the Perlin noise mechanism. I want to incorporate these principles of responsive element with random chaos while maintaining visual coherence. The aim is create something that feels alive and unpredictable but not 'ugly' or broken.

## Part 2: Coding Technique Exploration

! [An image of the code refer 1](Assets/PerlinNoise.png)
_Fig 2: Live sketch. perlin noise_

Link to refernce 1: https://genekogan.com/code/p5js-perlin-noise/


! [An image of the code refer 1](Assets/Random.png)
_Fig 3: Driving position and colour_

Link to reference 2: https://editor.p5js.org/codingtrain/sketches/vDcIAbfg7

The specific technique is 3D Perlin noise sampling in p5.js using noise(x, y, time). Using these two arguments I can map to canvas coordinates and the third increments each frame to produce animation.Each shape on the canvas has a position, rotation and size, which will recieve a smooth varying offset from the noise field. This will produce an organic displacement seen in the Spiderverse. Additionally, the mouse coordinates can be fed into noise inputs so the viewer actively warps the field in real time. This is different from random() because Perlin noise guarantees continuity by basing of neibouring values hence the motion feels fluid and not shakey.

