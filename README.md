# Numerical Computing in Modern C++ — Portfolio Project

Production-style implementations of core numerical analysis in **C++17**:
object-oriented design, **interpolation**, **differentiation**, **integration**, and **ODE** solving (RK4),
framed as practical analytics components (tracking, energy, ballistics).

## Modules (mapped from original questions)
- **OOP Foundations** (`src/oop_foundations/`) — player/team classes, ability metrics, state updates.
- **Tracking & Kinematics** (`src/tracking_kinematics/`) — coordinate transforms, centred differences for v(t)/a(t), speed series export.
- **Energy via Interpolation & Integration** (`src/energy_integration/`) — Lagrange interpolation P(v), composite trapezoid & Newton–Cotes 4-point.
- **Ballistics with RK4** (`src/ballistics_rk4/`) — 6-state ODE; gravity, drag, Magnus (switchable); multi-speed runs and outcomes.

The original brief is kept in `docs/` for context; this repository presents a professional, modular implementation.

## Structure
.
├── src/
│   ├── oop_foundations/
│   ├── tracking_kinematics/
│   ├── energy_integration/
│   ├── ballistics_rk4/
│   └── common/               # interpolation, RK4, shared utils
├── include/
├── data/                      # raw inputs (git-ignored outputs)
├── docs/                      # PDF brief(s)
├── report/figures/            # generated plots (git-ignored)
├── CMakeLists.txt
└── README.md

## Build (macOS/Linux)
mkdir -p build && cd build
cmake ..
cmake --build . -j

## Run
./oop_foundations
./tracking_kinematics
./energy_integration
./ballistics_rk4 25

## Tech
C++17 · CMake · STL · Lagrange/ Newton interpolation · Newton–Cotes · RK4

## License
MIT
# C-Project
