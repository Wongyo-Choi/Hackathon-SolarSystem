# Solar System Simulation Web Application

This repository contains a single-page web application that renders an interactive simulation of the solar system using Three.js. It also features an FAQ overlay that users can toggle via the top navigation bar.

---

## Overview

The application displays the Sun, Earth (with its Moon and clouds), and the major planets of the solar system, each following an elliptical orbit. The scene is rendered in 3D using WebGL, with real-time animations for planetary rotations and orbits. A dynamic FAQ overlay, which is accessible from the top bar, provides additional information when required.

---

## Features

- **Interactive 3D Simulation:**  
  Visualises the solar system with detailed textures and animations, utilising Three.js and OrbitControls for smooth user interaction.

- **Real-Time Animation:**  
  Updates the positions and rotations of celestial bodies in real time to simulate orbital mechanics and planetary spins.

- **FAQ Overlay:**  
  An easily accessible overlay is integrated via an iframe that can display an external FAQ page. The overlay can be toggled on or off using a dedicated button.

- **Responsive User Interface:**  
  A fixed top bar provides navigation with a title and an FAQ button, ensuring the interface remains uncluttered.

---

## Technologies Used

- **HTML5 & CSS3:**  
  For structuring and styling the web application.

- **JavaScript (ES6 Modules):**  
  Contains the core logic for the simulation and user interactions.

- **Three.js:**  
  A powerful library used to create and render the 3D solar system scene.  
  - Modules are imported from:  
    `https://web.cs.manchester.ac.uk/three/three.js-master/build/three.module.js`  
  - OrbitControls are used for camera manipulation.

- **WebGL:**  
  Enables hardware-accelerated 3D rendering in the browser.

---

## How to Use

1. **Download or Clone the Repository:**  
   Ensure you have the latest version of the files.

2. **Ensure Internet Connectivity:**  
   The application loads textures and Three.js modules from external URLs, so an active internet connection is necessary.

3. **Open the HTML File:**  
   Open the main HTML file (e.g., `index.html`) in a modern web browser. The simulation should start automatically.

4. **Interact with the Simulation:**  
   - Use your mouse or touch gestures to pan, zoom, and rotate the scene.
   - Click the **FAQ** button in the top bar to display the FAQ overlay.
   - Click the close icon (&times;) on the overlay to dismiss it.

---

## File Structure

- **index.html:**  
  Contains the complete HTML, CSS, and JavaScript for the simulation and FAQ overlay.

- **External Assets:**  
  The application utilises remote texture assets (e.g., for the Sun, Earth, Moon, and other planets) and external modules for Three.js. No local asset files are required.

---

## Customisation

- **FAQ Page:**  
  To change the FAQ content, update the `src` attribute of the `<iframe>` element in the FAQ overlay section.

- **Simulation Parameters:**  
  Modify values such as rotation speeds, orbital periods, and the scaling of celestial bodies directly in the JavaScript code to tailor the simulation.

- **Styling:**  
  Adjust the inline CSS in the `<style>` section to change the appearance of the top bar, overlay, and other elements.
