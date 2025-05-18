# ✈️ A320 Takeoff Simulation

This project simulates the takeoff roll of an Airbus A320 using basic physics principles and numerical integration (Euler method). It visualizes key dynamics including velocity, acceleration, drag, and thrust over time.

## 📊 Features

- Simulates aircraft acceleration from rest under constant thrust and quadratic drag.
- Compares actual (drag-affected) velocity with ideal (no-drag) motion.
- Visualizes:
  - Velocity vs. time
  - Acceleration vs. time
  - Drag vs. thrust over time using dual-axis plots

## 📁 Project Structure

```
├── takeoff_simulation.ipynb   # Main simulation and plotting notebook
├── README.md                  # Project documentation
```

## ⚙️ Physics Model

The simulation uses the following assumptions and equations:

- **Thrust (T)**: Constant force from engines.
- **Drag (D)**: Quadratic drag model → \( D = k \cdot v^2 \)
- **Newton’s Second Law**: \( a = \frac{T - D}{m} \)
- Numerical integration with Euler’s method to compute velocity and position.

## 🚀 Getting Started

### Prerequisites

Make sure you have Python installed with the following packages:

```bash
pip install numpy matplotlib moviepy
```

> **Note:** `moviepy` is included for potential video extensions but is not used in the current script.

### Running the Simulation

1. Open the notebook in Jupyter:

   ```bash
   jupyter notebook takeoff_simulation.ipynb
   ```

2. Run all cells to execute the simulation and generate plots.

## 📈 Example Output

- **Velocity Plot:** Shows simulated vs. ideal velocity, including takeoff threshold.
- **Acceleration Plot:** Highlights decreasing acceleration as drag increases.
- **Drag vs. Thrust:** Demonstrates how drag grows over time and approaches thrust.

## ✍️ Author

- [Your Name](https://github.com/AIMLExperimentsAndMore)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
