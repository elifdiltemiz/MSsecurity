# Security of Mobile Systems

### University of Regensburg | Erasmus+ Internship Projects

---

## Class Exercises – Google Colab

- [Notebook 1 (Lecture)](https://colab.research.google.com/drive/1W5aDUaIQ_47uETDXh200sRXYa0FV0nGY?usp=sharing)
- [Notebook 2 (Free Space)](https://colab.research.google.com/drive/1LUyPkr8dMVcj5Ae7P8FwbMzOYEPP7vzQ?usp=sharing)
- [Notebook 3 (Munich)](https://colab.research.google.com/drive/1qpT4WgVkXUd4duRsOmcp6O93rB9HMoUI?usp=sharing)

---

## About This Repository

This repository documents practical exercises, technical implementations, and simulation-based projects developed during an **Erasmus+ internship at the University of Regensburg, Germany**.

The work focuses on **wireless communication, radio signal propagation, and mobile system security**, combining theoretical concepts with practical experiments and Python-based simulations.

### Wireless Communication and Radio Propagation

This repository collects our work with NVIDIA Sionna RT, a ray-tracing library for simulating radio wave propagation. It includes installation resources that explain how to set up Sionna RT locally and in Google Colab, and interactive Jupyter Notebooks starting with detailed fundamentals in which simple scenes with a base station, receivers, and buildings are built step by step.

Each notebook is organized around research questions: we first state the question, then run the simulation, and finally explain the results. The experiments examine how the received signal strength (RSS) and path gain depend on distance, frequency, obstacles, and building materials, and how reflection, refraction, and diffraction shape the signal that reaches the receiver.

The results are compared with theoretical models such as the free-space path loss formula and visualized with plots and 3D scene previews, so that effects like shadowing, material losses, and multipath interference become directly visible.

### Mobile Network Security and Encryption

In addition to wireless propagation studies, the repository includes GSM security notebooks focusing on mobile network authentication, cryptographic algorithms, and encryption mechanisms.

The notebooks combine theoretical explanations, educational cryptographic models, historical algorithm implementations, and Python-based simulations. They explore A3/A8 authentication and key generation, A5 encryption algorithms, COMP128-1, LFSR-based encryption, IMSI/TMSI privacy, and mobile network vulnerabilities.

The experiments also examine IMSI catcher and downgrade attacks, protocol-level security weaknesses, and security improvements introduced from GSM (2G) to UMTS (3G).

---

## Project Overview

The repository is organized into topic-based folders covering different aspects of wireless communication systems and related technologies.

Each folder provides relevant documentation, implementations, or experimental work. Additional projects and research activities can be integrated into this structure as the work progresses.

| Project | Description | Documentation |
|---|---|---|
| **Sionna RT Installation** | Installation and environment setup for Sionna RT on Windows, Linux, and macOS, including installation scripts and setup exercises. | [View Installation Guide](install/README.md) |
| **01 - Wireless Fundamentals** | Frequency, wavelength, free-space path loss (FSPL), and received power calculations. | [View Notebook](sionna-rt/Project-01-Wireless-Fundamentals/SMS_Exercise1_Revised_Student.ipynb) |
| **02 - Building Effects** | Investigation of building obstructions, concrete and wood materials, and their effects on received signal strength (RSS). | [Basic Notebook](sionna-rt/Project-02-Building-Effects/building_effects.ipynb) / [Research Questions](sionna-rt/Project-02-Building-Effects/researchQAs.ipynb) |
| **03 - Multipath Propagation** | Reflection, diffraction, scattering, LOS/NLOS comparisons, and propagation mechanism analysis using Sionna RT. | [Basic Notebook](sionna-rt/Project-03-Multipath-Propagation/multipathPropagation.ipynb) / [Research Questions](sionna-rt/Project-03-Multipath-Propagation/Research_Questions.ipynb) |
| **04 - GSM Security Fundamentals** | GSM security architecture, authentication, A3/A8 algorithms, encryption mechanisms, and subscriber identity protection through interactive exercises and educational implementations. | [View Notebook](GSM/GSM_Security_Notebook.ipynb) |
| **05 - GSM Encryption and Security Analysis** | Historical COMP128-1 and A5/1 implementations, LFSR-based encryption, IMSI catcher and downgrade attack simulations, and GSM/UMTS security comparisons. | [View Notebook](GSM/Notebook2.ipynb) |

---

## Technologies and Tools

The projects use a combination of programming languages, simulation frameworks, and development environments.

- **Python** - Programming, numerical calculations, cryptographic implementations, and simulation analysis.
- **Jupyter Notebook** - Interactive coding, explanations, and experimental documentation.
- **NVIDIA Sionna RT** - Ray-tracing-based wireless propagation simulations.
- **Mitsuba 3** - 3D scene representation and rendering.
- **NumPy** - Numerical computations and array operations.
- **Matplotlib** - Data visualization, message sequence diagrams, and graphical analysis.
- **Google Colab / VS Code** - Development and execution environments.

---

## Research Focus

The work combines theoretical knowledge with practical implementations to explore different aspects of wireless communication and mobile systems.

Through computational exercises and simulation-based experiments, the projects investigate signal propagation behavior, wireless communication characteristics, and the influence of environmental conditions on radio signals.

The security-related projects focus on GSM authentication, session key generation, encryption, cryptographic algorithms, subscriber identity protection, protocol vulnerabilities, and the evolution of mobile network security from 2G to 3G.

---

## Repository Structure

```text
MSsecurity/
│
├── GSM/
│   ├── GSM_Security_Notebook.ipynb
│   └── Notebook2.ipynb
│
├── install/
│   ├── exercise.ipynb
│   ├── Linux.sh
│   ├── macOS.sh
│   ├── README.md
│   └── Windows.ps1
│
├── sionna-rt/
│   │
│   ├── Project-01-Wireless-Fundamentals/
│   │   └── SMS_Exercise1_Revised_Student.ipynb
│   │
│   ├── Project-02-Building-Effects/
│   │   ├── building_effects.ipynb
│   │   └── researchQAs.ipynb
│   │
│   └── Project-03-Multipath-Propagation/
│       ├── multipathPropagation.ipynb
│       └── Research_Questions.ipynb
│
└── README.md
```

---

## How to Use

### 1. Clone the Repository

Clone the repository to your local computer using Git:

```bash
git clone https://github.com/elifdiltemiz/MSsecurity.git
cd MSsecurity
```

Open the downloaded repository in **VS Code** or **JupyterLab**.

### 2. Set Up the Environment

For Sionna RT installation and environment configuration, refer to the [Installation Guide](install/README.md).

The installation folder provides platform-specific scripts and supporting resources for:

- **Windows**
- **Linux**
- **macOS**

### 3. Explore the Projects

Navigate to a project folder and open the corresponding Jupyter Notebook.

Run the notebook cells sequentially to explore the theoretical explanations, Python implementations, simulations, visualizations, and experimental results.

The GSM security notebooks can be explored independently of Sionna RT. All security simulations are intended for educational and research purposes.

### Requirements

Software dependencies depend on the selected project.

- **Basic computational exercises:** Python, NumPy, and Matplotlib.
- **Ray-tracing simulations:** NVIDIA Sionna RT and its compatible dependencies.
- **GSM security exercises:** Python and the additional dependencies specified in the corresponding notebooks.

---

## Authors and Contact

This repository was developed collaboratively during an **Erasmus+ internship at the University of Regensburg**.

### Elif Diltemiz

- **Email:** diltemizeliff@gmail.com

  
### Zehra Özcan

- **Email:** zehra12ozcn@gmail.com

---

## Acknowledgment

We would like to thank the **University of Regensburg** for providing the opportunity to explore wireless communication and mobile system security through practical exercises, technical implementations, and simulation-based research during our Erasmus+ internship.

---

**University of Regensburg | Erasmus+ Internship | 2026**
