# Human Gaze Perception Bias Simulation using Bayesian Networks

This project simulates and visualizes how humans perceive gaze direction under varying levels of noise, inspired by the cognitive psychology study **"Humans Have an Expectation That Gaze Is Directed Towards Them."** Using Bayesian Networks, the project models how humans interpret gaze based on **pupil orientation**, **head orientation**, and **noise level**.

## Cognitive Robotics Context

Understanding how humans perceive gaze under uncertainty has strong implications for cognitive robotics. Robots interacting with humans can benefit from incorporating or understanding such perceptual biases, enabling more natural and intuitive human-robot interaction.

---
## Experiments

### Experiment 1: Pupil Orientation + Noise
- Simulates perception of gaze (`towards` vs `away`) under three noise levels: low, medium, high.
- Uses a **bias model** based on observed pupil orientation.

| Noise Level | If Observed = "towards" | If Observed = "away" |
|-------------|--------------------------|------------------------|
| Low         | 0.9 towards / 0.1 away   | 0.3 towards / 0.7 away |
| Medium      | 0.95 / 0.05              | 0.5 / 0.5              |
| High        | 0.98 / 0.02              | 0.7 / 0.3              |

### Experiment 2: Head Orientation + Pupil + Noise
- Adds head orientation (-30° to 30°) as an additional variable.
- Models how humans rely more on **head orientation** when eye cues are noisy.

---
##  Conclusion

This project demonstrates how cognitive biases—like assuming gaze is directed at the observer—can be modeled computationally. For robots, such models offer twofold value: simulating human-like perception, or making objective decisions that account for human biases. This helps build more socially intelligent robotic systems.

---

## Tech Stack

- Python
- `pgmpy` for Bayesian modeling
- `pandas`, `numpy` for data
- `matplotlib`, `seaborn`, `networkx` for visualization

---

## License

MIT License

---

## Author

Developed as part of the **Cognitive Robotics** module in an MSc Artificial Intelligence program.
