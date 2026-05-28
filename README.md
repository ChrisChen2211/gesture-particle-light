Gesture Particle Light Interaction

A browser-based interactive particle light effect controlled by real-time hand gestures. The project uses the webcam to detect hand movements and changes the particle system according to different gestures, creating a futuristic visual interaction experience.

Project Overview

This project is an experimental web interaction demo that combines hand tracking, particle animation, and light effects. After the user allows camera access, the webpage captures hand landmarks in real time and classifies simple hand gestures. Each gesture triggers a different particle behaviour, such as expansion, contraction, vortex movement, laser scanning, and core collapse.

The main goal of this project is to create a visually engaging interface where users can control digital particles through natural hand movements instead of using a mouse or keyboard.

Main Features

Real-time Hand Tracking

The webpage uses the user’s webcam to detect hand position and hand landmarks in real time. The detected palm position becomes the main control point for the particle system.

Gesture-based Particle Reactions

Different hand gestures create different visual effects:

Gesture	Particle Effect
Open palm	Particles burst outward with ripple effects
Fist	Particles collapse toward the hand position
Pinch	Particles strongly compress into a bright core
One finger	A laser scanning beam appears across the particle field
Two fingers	Particles form a twin vortex movement
No hand detected	Particles return to ambient floating mode

Light and Motion Effects

The project includes several visual effects to make the interaction more dynamic:

* Particle motion trails
* Expanding ripple rings
* Spark burst effects
* Hand aura glow
* Laser scan line
* Twin vortex guide rings
* Core collapse animation
* Animated radial background lighting

Performance Optimisation

The first version used a large number of particles and heavy glow rendering. The updated version improves performance by:

* Reducing the number of particles
* Avoiding expensive radial gradients for every particle
* Using motion trails instead of heavy glow rendering
* Lowering hand tracking model complexity
* Reducing webcam input resolution
* Limiting the number of spark particles

These changes make the animation smoother while still keeping the visual effect strong.

Technologies Used

* HTML5
* CSS3
* JavaScript
* Canvas API
* MediaPipe Hands
* Webcam API

How to Run

Option 1: Run with VS Code Live Server

1. Create a project folder.
2. Save the webpage code as index.html.
3. Open the folder in VS Code.
4. Install the Live Server extension.
5. Right-click index.html and select Open with Live Server.
6. Click Start Hand Tracking on the webpage.
7. Allow camera permission in the browser.

Option 2: Run with Localhost

You can also run the page through any local development server. For example, if Python is installed, open the project folder in Terminal and run:

python3 -m http.server 5500

Then open the following address in your browser:

http://localhost:5500

Important Notes

Camera access may not work if the file is opened directly with file://. It is recommended to run the page using Live Server or localhost.

For best performance, use a modern browser such as Google Chrome, Microsoft Edge, or Safari. A well-lit environment also helps improve hand tracking accuracy.

Interaction Design

The interaction is designed around natural hand movement. Instead of clicking buttons, the user controls the particle field by changing hand gestures. This creates a more immersive and futuristic experience.

The palm position is used as the central point of interaction. When the user moves their hand, the particles follow or react around that position. The gesture type then determines how the particles behave.

For example, when the user opens their hand, the particles expand outward like an energy burst. When the user makes a fist, the particles contract toward the hand as if being pulled by gravity. When the user pinches their fingers, the particles collapse into a bright core.

File Structure

GestureParticleDemo/
├── index.html
└── README.md

Possible Future Improvements

* Add support for two-hand interaction
* Add sound effects based on gesture changes
* Add custom colour themes
* Add screenshot or recording function
* Add more gesture types
* Add UI controls for particle density and speed
* Convert the project into a React version

Author

Created as an interactive web visualisation project using hand gesture recognition and canvas-based particle animation.
