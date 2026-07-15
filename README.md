# ❄️ Winter Night Village using OpenGL

An interactive 2D winter village simulation developed using **OpenGL** and **GLUT** in **C++**. The project recreates a snowy mountain village with animated cable cars, continuous snowfall, moonlit scenery, and interactive house lighting. It demonstrates fundamental computer graphics concepts including geometric modeling, hierarchical object construction, particle systems, Bezier curve animation, event handling, and the Painter's Algorithm.

---

## 📌 Project Overview

This project was developed as part of the **CSE-4202 Computer Graphics Lab** course.

The objective was to design and implement a complete 2D animated environment using only OpenGL primitives without relying on external graphics engines. Every object in the scene was manually constructed by defining vertex coordinates inside an orthographic coordinate system.

The scene consists of:

- Snow-covered mountains
- Multiple village houses
- Pine trees
- Animated cable cars
- Continuous snowfall
- Moonlit night sky
- Interactive house lighting

The project combines static scene rendering with real-time animation and user interaction to simulate a dynamic winter environment.

---

## ✨ Features

- ❄️ Continuous snowfall using a particle system (500+ snowflakes)
- 🚠 Animated cable cars moving along quadratic Bezier curves
- 🌙 Moonlit winter night environment
- 🏠 Interactive house lighting controlled with mouse clicks
- 🌲 Hierarchical tree modeling
- 🏔️ Polygon-based mountain rendering
- 🎨 Painter's Algorithm for correct rendering order
- 🖱️ Mouse event handling using ray-casting polygon detection
- ⚡ Smooth animation at approximately 60 FPS

---

## 🖼️ Scene Components

The winter village is constructed entirely from OpenGL geometric primitives.

| Component | Primitive Used |
|------------|----------------|
| Sky | Polygon |
| Mountains | Multiple Polygons |
| Moon | Circular Polygon |
| Houses | Rectangles + Triangles + Polygons |
| Trees | Rectangles + Multiple Triangles |
| Cable Lines | Quadrilateral Polygons |
| Cable Cars | Trapezoids + Rectangles + Lines |
| Snow Ground | Irregular Polygons |
| Snowflakes | Circular Polygons |

---

## 📐 Coordinate System

The scene is rendered using a 2D orthographic projection:

```cpp
gluOrtho2D(-24, 24, -14, 14);
```

Coordinate Range

- X-axis: **-24 to 24**
- Y-axis: **-14 to 14**

All scene objects were first planned on a Cartesian coordinate grid before implementation, allowing consistent positioning and scaling throughout the environment.

---

## 🧮 Computer Graphics Concepts Used

This project demonstrates several core computer graphics concepts, including:

- Geometric Modeling
- Orthographic Projection
- Hierarchical Object Construction
- Polygon Rendering
- Affine Translation
- Quadratic Bezier Curve Animation
- Particle System Animation
- Event-Driven Programming
- Mouse Interaction
- Ray-Casting Polygon Detection
- Double Buffering
- Timer-Based Animation
- Painter's Algorithm

---

## ⚙️ Technologies Used

- **Programming Language:** C++
- **Graphics Library:** OpenGL
- **Toolkit:** GLUT (FreeGLUT)
- **Compiler:** GCC (MinGW)
- **IDE:** Code::Blocks 20.02
- **Operating System:** Windows 10/11

---

## 📂 Project Structure

```
winter-night-village-opengl/
│
├── assets/
│   └── coordinate_plot.png
│
├── docs/
│   └── Winter_Night_Village_OpenGL_Report.pdf
│
├── screenshots/
│   ├── complete_scene.png
│   ├── snowfall_animation.png
│   ├── cable_car_animation.png
│   └── interactive_house_lighting.png
│
├── src/
│   └── main.cpp
│
├── README.md
└── LICENSE
```

---

## 📸 Screenshots

### Complete Winter Scene

> *(Add complete_scene.png here)*

---

### Snowfall Animation

> *(Add snowfall_animation.png here)*

---

### Cable Car Animation

> *(Add cable_car_animation.png here)*

---

### Interactive House Lighting

> *(Add interactive_house_lighting.png here)*

---

### Coordinate Plot

> *(Add coordinate_plot.png here)*

---

## ▶️ How to Run

### Clone the repository

```bash
git clone https://github.com/yourusername/winter-night-village-opengl.git
```

### Compile

```bash
g++ main.cpp -o winter_village -lglut -lGLU -lGL
```

### Run

```bash
./winter_village
```

---

## 🖱️ Controls

| Input | Function |
|--------|----------|
| Left Mouse Click | Toggle house light ON/OFF |

---

## 📊 Performance

| Metric | Value |
|---------|-------|
| Frame Rate | ~60 FPS |
| Snow Particles | 500+ |
| Cable Cars | 3 |
| Rendering Technique | Double Buffering |
| Coordinate System | Orthographic Projection |

---

## 🚀 Future Improvements

Possible extensions for the project include:

- 3D scene rendering
- Dynamic weather effects
- Day–night transition
- Texture mapping
- Shader-based lighting
- Sound effects
- Camera movement
- Additional interactive elements

---

## 👩‍💻 Author

**Nadia Afroj Orin**

Bachelor of Science in Computer Science and Engineering

Notre Dame University Bangladesh

GitHub: https://github.com/yourusername

---

## 📄 License

This project is intended for educational and learning purposes.
