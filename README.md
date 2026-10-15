# Welcome to Qompute 2026!
All Challenges are provided by IBM Quantum and to be completed with Qiskit. 

> [!IMPORTANT]
**Please note that in-person attendees must check in on 10/18, contact qee@usc.edu for any concerns**

- [Overview](#overview)
- [How to Start Qomputing](#how-to-start-qomputing)
- [Final Submission Due Date](#final-submission-due-date)
- [Challenge Tracks](#challenge-tracks)
- [Judging Criteria](#judging-criteria)
- [Submission Details and Challenges](#submission-details-and-challenges)
- [Winners](#-winners-)
- [Feedback](#Feedback)
------

## **Overview**

There are multiple challenge tracks, and it is up to you and your teammates to work on one or multiple challenges. Your goal is to present a project that responds to the challenge and aligns with the [judging criteria](#judging-criteria) listed below.

This QEE hackathon is part of IBM Quantum's Qiskit Fall Fest this year, it is our pleasure to work alongside many other universities around the world in an effort to enhance quantum computing education and strengthen the quantum ecosystem in LA. [Check out Qiskit Fall Fest's page for more details, if you are interested!](https://www.ibm.com/quantum/events/fall-fest-2026)

### A Decade of Quantum in the Cloud

In May 2016, IBM made a five-qubit quantum processor available through the cloud, giving people outside specialized research laboratories the opportunity to program real quantum hardware from a browser. Ten years later, quantum processors contain far more qubits, operations have become more reliable, and increasingly sophisticated software allows researchers to run larger and more complex experiments than was possible on that first device.

One of the most promising applications is the simulation of quantum systems, including molecules, materials, and many-body physics. These problems are especially well suited to quantum computing because nature and quantum computers obey the same quantum-mechanical rules. A quantum computer can therefore represent certain states and interactions more directly than a classical computer can. This does not make these problems easy, but it offers a compelling path toward studying phenomena that become extraordinarily difficult to model as their complexity grows.

Today's quantum computers remain noisy, limited in the size and duration of the calculations they can perform, and expensive to build and operate. Most current results are still research experiments rather than solutions to large, practical problems. However, cloud access has opened the field to many more people! [1]

The gap between quantum computing's potential and its present-day reality is where this hackathon begins. This year's theme is **A Decade of Quantum in the Cloud: Who Does It Serve?** Each track asks you to use Qiskit to explore a real-world problem *and* to think critically about the people, communities, and systems your work could affect. You are not expected to solve quantum computing in a single hackathon. Instead, we invite you to experiment boldly, question assumptions, and imagine how this technology might develop and who should benefit when it does.

- **[Track 1 — Molecules for a Livable Planet](#track-1-molecules-for-a-livable-planet):** Use quantum simulation to investigate a molecule or simplified chemical process related to food, clean energy, or sustainable materials.
- **[Track 2 — Optimizing for People](#track-2-optimizing-for-people):** Formulate a problem involving scarce resources, scheduling, or logistics as a quantum optimization task. Examine who defines the objective, which constraints matter, and who might be left out.
- **[Track 3 — Can We Trust a Noisy Quantum Computer?](#track-3-can-we-trust-a-noisy-quantum-computer)** Design experiments that measure noise, compare hardware or error-handling methods, and determine what evidence is needed before a quantum result should be trusted.

> [!NOTE]
> All quantum components must be built and run with Qiskit (circuits, transpilation, primitives, and Qiskit add-ons). Classical helper libraries such as PySCF, NumPy, and SciPy are allowed for the classical parts of your workflow. Running on real IBM hardware is welcome but not required, a well-analyzed simulator project can win. Keep in mind that all USC students get 10 minutes of free computing time on IBM hardware so you can choose to take advantage of that!

## **How to Start Qomputing**

[Start Here: How to Install Qiskit and Make Yourself ready for this Hackathon](https://docs.google.com/document/d/12Be_4zIUcz8xkC1jnlbSwCfLch4eiJhVqtn0Syusv70/edit?usp=sharing)

[Quantum Learning Resources](https://drive.google.com/drive/folders/1h8H3HqeEugLJRGnizbYnJ-sTYo3oBGBV?usp=sharing)

Please visit [IBM Setup Guide](https://docs.google.com/document/d/12Be_4zIUcz8xkC1jnlbSwCfLch4eiJhVqtn0Syusv70/edit?usp=sharing) for an overview of installing Qiskit, accessing the online environment, and using the backend computing tools.

### Access to IBM Hardware
Whether you will work locally or in a cloud environment, the first step for all users is to install Qiskit. Please visit [IBM Qiskit install guide](https://quantum.cloud.ibm.com/docs/en/guides/install-qiskit) to learn about how to install Qiskit and set up the Python environment.

Also, you can visit this YouTube videos: [How to Install Qiskit | Coding with Qiskit 1.x | Programming on Quantum Computers](https://youtu.be/dZWz4Gs_BuI?si=um36GxYPqrcAaZC_)


### Using an Online Environment
To ensure an easy and consistent experience for all participants—especially those on Windows — we can try [qBraid](https://www.qbraid.com/), one of the supported online environments, to provide a pre-configured, ready-to-use environment to use Qiskit. You can follow these steps to launch the lab notebooks on qBraid.

You can find [detailed instructions](https://docs.qbraid.com/lab/user-guide/getting-started) on qBraid.

📎 Learn more and get started here: [IBM Quantum Online Lab Environments Guide](https://quantum.cloud.ibm.com/docs/en/guides/online-lab-environments)

## Final Submission Due Date

> [!IMPORTANT]
Submission Due: 11:59PM PST, 14th Oct (Wednesday)</br>
Link will expires after due, please turn in your project on time [using this link](https://docs.google.com/forms/d/e/1FAIpQLSffK6jWlW7L8uXGhQ_336lzX1qnckdqiC-M593KWLag3hKDBw/viewform?usp=dialog)

## Challenge Tracks

### Track 1: Molecules for a Livable Planet

This track is for participants who want to use quantum computers for what Feynman originally imagined them for: simulating nature itself.

#### Quantum Chemistry and Global Challenges

Some of humanity's most urgent problems are, at their core, chemistry problems. The Haber-Bosch process that makes fertilizer for roughly half the world's food supply consumes about 1–2% of global energy, because breaking nitrogen's triple bond is so difficult. Better batteries, cleaner hydrogen fuel, and materials that capture carbon dioxide all depend on understanding how electrons behave inside molecules. Classical computers struggle with exactly these situations especially when bonds stretch and break, where simple approximations like Hartree-Fock fail badly. [2]

Quantum algorithms such as the Variational Quantum Eigensolver (VQE) and Sample-based Quantum Diagonalization (SQD) offer a path forward. SQD in particular has powered some of the largest chemistry experiments ever run on IBM quantum hardware, by letting the quantum computer propose important electron configurations and a classical computer solve within them. [3], [4]

#### Your Challenge: Simulate a molecule that matters

Choose a molecule (or a simplified model of one) connected to a real-world problem, and use Qiskit to compute a property that tells you something meaningful about it. Your goal is to:

1. Select a molecule and explain why it matters to people or the planet.
2. Identify a chemical property to investigate (e.g., ground-state energy, a bond-dissociation curve, the effect of stretching a bond).
3. Implement the simulation using Qiskit and appropriate classical chemistry software.
4. Compare against classical reference methods and interpret your results, including their limitations, in the context of the molecule's application.

#### Start from here

- **Feeding the World:** N₂'s triple bond is what makes fertilizer production so energy-intensive. Can you show how the difficulty of describing N₂ changes as the bond is stretched, and compare how classical and quantum-assisted methods handle it?
- **Clean Hydrogen:** Hydrogen is a promising zero-carbon fuel. Can you compute the dissociation curve of H₂ (or HeH⁺) and explain where simple methods break down and why that matters for modeling fuel chemistry?
- **Better Batteries:** Lithium-containing molecules like LiH are simple models for battery chemistry. How small can you make your quantum resources (qubits, circuit depth) while still reaching chemical accuracy?
- **Your Own Molecule:** Pick a small molecule related to pollution, medicine, or materials and justify why a quantum approach is (or isn't yet) the right tool.

#### Think about the impact

- Who would benefit if quantum chemistry delivered better fertilizers, batteries, or drugs; who might be left out of the benefits?
- Chemistry knowledge can be dual-use. Are there risks in making molecular simulation more powerful?
- Quantum and classical computing both consume energy. Is the computational cost of your approach justified by what it reveals?
- How confident can you honestly be in your result? What would you need before making a real-world claim?

#### Starter resources

All Track 1 files are in the [`Track 1`](Track%201) folder.

- SQD from scratch lab (notebooks 1–3): [`01_sample_then_diagonalize.ipynb`](Track%201/01_sample_then_diagonalize.ipynb), [`02_molecules_as_bitstrings.ipynb`](Track%201/02_molecules_as_bitstrings.ipynb), [`03_the_full_sqd_pipeline.ipynb`](Track%201/03_the_full_sqd_pipeline.ipynb)
- Ground-State Energy of a Molecule with VQE — [`challenge_1_tutorial_VQE.ipynb`](Track%201/challenge_1_tutorial_VQE.ipynb), B. Tirado, BasQ Qiskit Fall Fest 2026 (CC BY 4.0)

---

### Track 2: Optimizing for People

This track is for participants ready to explore one of the most promising near-term applications of quantum computers: solving complex optimization problems and questioning what we choose to optimize.

#### Quantum Optimization and Real Decisions

Every day, organizations decide how to split limited resources: which clinics get vaccine shipments, which neighborhoods get new transit routes, which projects a city funds, which assets a pension fund holds. These are optimization problems with constraints, and as the number of choices grows, the number of possible solutions explodes beyond what any computer can check one by one.

The Quantum Approximate Optimization Algorithm (QAOA) encodes a problem's cost into a quantum Hamiltonian and searches for low-cost solutions using alternating quantum layers tuned by a classical optimizer. [5], [6] Real problems have rules: budgets, capacities, "pick exactly K", and folding those constraints into the quantum problem is where encoding becomes an art. [7] However, an optimized solution is only as good as its objective function: the numbers you choose to reward and penalize are value judgments.

#### Your Challenge: Solve a real allocation problem and defend your objective

Choose a real-world resource-allocation or decision problem with at least one constraint, formulate it as a cost function, and use QAOA (or a variant) in Qiskit to find good solutions. Your goal is to:

1. Frame a concrete scenario and explain who the decision affects.
2. Translate it into a cost Hamiltonian, including your constraint(s) as a penalty.
3. Solve it with Qiskit and verify your answer against a brute-force or classical solution on a small instance.
4. Reflect on how the choices in your cost function (weights, penalties, what is left out) shape the "optimal" outcome.

#### Start from here

- **Sustainable Investing:** Choose K assets from a small universe to balance expected return against risk, then add a sustainability or ESG score. How does changing that weight change the portfolio?
- **Fair Aid Distribution (Knapsack):** Allocate a limited relief budget across projects, each with a cost and an impact score. What happens when "impact" is measured differently for different communities?
- **Power Grid or Community Planning (Max-Cut):** Partition a network of neighborhoods, substations, or social groups. What does a "maximum cut" mean for the people on either side of it?
- **Scheduling for Equity:** Assign limited time slots (clinic appointments, exam rooms, shifts) under constraints. Can your formulation include fairness, not just efficiency?

#### Think about the impact

- Who chose the objective function, and whose priorities does it encode?
- Could an "optimal" solution systematically disadvantage a group? How would you detect that?
- When should an algorithm make an allocation decision, and when should a human?
- If quantum optimization becomes faster than classical methods, who gets access to that advantage first?

#### Starter resources

All Track 2 files are in the [`Track 2`](Track%202) folder.

- Combinatorial Optimization with QAOA: Max-Cut — [`Track2_challenge_2_tutorial.ipynb`](Track%202/Track2_challenge_2_tutorial.ipynb), B. Tirado, BasQ Qiskit Fall Fest 2026 (CC BY 4.0)
- [Quantum approximate optimization algorithm (IBM tutorial)](https://quantum.cloud.ibm.com/docs/tutorials/quantum-approximate-optimization-algorithm) — end-to-end QAOA in Qiskit
- [Portfolio optimization tutorial (Qiskit Finance)](https://qiskit-community.github.io/qiskit-finance/tutorials/01_portfolio_optimization.html) — a budget-constrained selection problem
- [Converters for quadratic programs (Qiskit Optimization)](https://qiskit-community.github.io/qiskit-optimization/tutorials/02_converters_for_quadratic_programs.html) — turning constraints into penalty terms
- [Max-Cut and Traveling Salesperson tutorial (Qiskit Optimization)](https://qiskit-community.github.io/qiskit-optimization/tutorials/06_examples_max_cut_and_tsp.html)
- [Warm-starting QAOA (Qiskit Optimization)](https://qiskit-community.github.io/qiskit-optimization/tutorials/10_warm_start_qaoa.html)

---

### Track 3: Can We Trust a Noisy Quantum Computer?

This track is your entry point into the hardware reality behind every quantum result: noise, connectivity, and the fight to get answers we can believe.

#### Ten Years of Noisy Quantum Computers

The 5-qubit processor IBM put on the cloud in 2016 was a milestone in access but its results were fragile. Today's processors have hundreds of qubits, yet every gate still carries a chance of error, and qubits can only interact directly with their neighbors. When a circuit needs two distant qubits to talk, the compiler inserts extra operations (SWAPs) that add even more noise. [8]

Researchers fight back in three ways: error suppression (designing circuits and layouts that avoid errors), error mitigation (statistically correcting noisy results after the fact), and error detection and correction (adding redundant qubits and checks that catch errors as they happen). [9], [10] Each comes with a cost, whether that is more gates, more qubits, or more discarded shots, and part of the craft is deciding whether that cost is worth paying.

#### Your Challenge: Make a quantum result more trustworthy

Choose a small quantum experiment, show how noise or hardware layout degrades it, and use Qiskit to make the result more reliable, then honestly report what that improvement cost. Your goal is to:

1. Pick an experiment with a known correct answer (e.g., an entangled Bell state, a small physics simulation, a simple algorithm).
2. Establish an ideal baseline and a noisy baseline (noise model, fake backend, or real hardware).
3. Apply at least one suppression, mitigation, or detection strategy.
4. Compare the improvement against its cost (extra gates, qubits, shots, or runtime) and explain what your results mean for people relying on quantum computers.

#### Start from here

- **Then vs. Now:** Create a Bell pair between two distant qubits on a 2016-style 5-qubit layout, a modern IBM-style layout, and a hypothetical alternative layout (such as a hyperbolic lattice). How do connectivity and routing change the quality of entanglement?
- **Catch the Error:** Add a simple parity or stabilizer check to a small circuit and keep only the shots that pass. How much does fidelity improve, and how many results do you throw away?
- **Rescue a Physics Simulation:** Simulate the magnetization of a small spin chain over time, then use error mitigation (e.g., zero-noise extrapolation, twirling, dynamical decoupling) to recover the curve that noise distorts.
- **Teach It as a Game:** Design a simple game or interactive demo in which players fight noise using error-detection or error-correction ideas, built on Qiskit circuits.

#### Think about the impact

- If a quantum computer's answer can't be fully verified, how should it be used in medicine, finance, or security decisions?
- Error correction may require thousands of physical qubits per useful qubit. Who will be able to afford fault-tolerant machines, and what happens to everyone else?
- Cloud access in 2016 opened quantum computing to students everywhere. Is access today more or less equal, and what would you change?
- How should researchers and companies communicate noisy results to the public without hype?

#### Starter resources

All Track 3 files are in the [`Track 3`](Track%203) folder.

- Geometry-aware quantum cloud challenge — [`Qiskit Fall Fest Challenge Hyperbolic Futures - quanTA USask.pdf`](Track%203/Qiskit%20Fall%20Fest%20Challenge%20Hyperbolic%20Futures%20-%20quanTA%20USask.pdf), S. Rayan, quanTA, University of Saskatchewan (Bell-pair architecture comparison)
- Simulating Quantum Dynamics: The Transverse-Field Ising Model — [`challenge_3_tutorial.ipynb`](Track%203/challenge_3_tutorial.ipynb), B. Tirado, BasQ Qiskit Fall Fest 2026 (CC BY 4.0)
- Gamifying Error Detection, Mitigation and Correction — [`McgillQFF 2026  -  Read-Only.pptx`](Track%203/McgillQFF%202026%20%20-%20%20Read-Only.pptx), W. Sun, McGill University
- [Error mitigation and suppression techniques (IBM guide)](https://quantum.cloud.ibm.com/docs/guides/error-mitigation-and-suppression-techniques)
- [Combine error mitigation options with the Estimator primitive (IBM tutorial)](https://quantum.cloud.ibm.com/docs/tutorials/combine-error-mitigation-techniques)
- [Transpile with pass managers (IBM guide)](https://quantum.cloud.ibm.com/docs/guides/transpile-with-pass-managers) — layouts, routing, and SWAP overhead

---

## Judging Criteria

1. **Technical Content - 35%:** Did you meet the technical requirements of your chosen track? Is your Qiskit implementation correct, and did you verify it against a reference or baseline?
2. **Societal Impacts - 20%:** How does your project connect to a real-world need, in the spirit of Responsible Innovation and engineering an ethical future in tech?
   - Did you consider the potential harms, limitations, or inequities of this technology?
   - Does your project make a clear and honest case for its positive impact?
3. **Presentation - 20%:** Comprehension, aesthetics, and delivery style. A good idea that cannot be shared cannot make an impact.
4. **Originality - 20%:** Creativity and problem solving. Is the project well researched, and did you go beyond the starter notebooks?
5. **Submitting correct and clean files and attendance/communication - 5%:**
   - Easy to follow and clean formatting on GitHub
   - Sources and references are included
   - *For all attendees:* You are responsible for your attendance; if someone from your team cannot come they should communicate with the organizers AND teammates. Teams who do not attend the conference on 10/18 without communication will be disqualified. 

## References

[1] World Economic Forum. 2024. *Quantum for Society: Meeting the Ambition of the SDGs.* Geneva, Switzerland: World Economic Forum.

[2] Reiher, Markus, Nathan Wiebe, Krysta M. Svore, Dave Wecker, and Matthias Troyer. 2017. "Elucidating Reaction Mechanisms on Quantum Computers." *Proceedings of the National Academy of Sciences* 114 (29): 7555–60.

[3] Robledo-Moreno, Javier, et al. 2025. "Chemistry Beyond the Scale of Exact Diagonalization on a Quantum-Centric Supercomputer." *Science Advances.* arXiv:2405.05068.

[4] Kandala, Abhinav, et al. 2017. "Hardware-Efficient Variational Quantum Eigensolver for Small Molecules and Quantum Magnets." *Nature* 549: 242–46.

[5] Farhi, Edward, Jeffrey Goldstone, and Sam Gutmann. 2014. "A Quantum Approximate Optimization Algorithm." arXiv preprint arXiv:1411.4028.

[6] Hadfield, Stuart, Zhihui Wang, Bryan O'Gorman, Eleanor G. Rieffel, Davide Venturelli, and Rupak Biswas. 2019. "From the Quantum Approximate Optimization Algorithm to a Quantum Alternating Operator Ansatz." *Algorithms* 12 (2): 34.

[7] Barkoutsos, Panagiotis Kl., Giacomo Nannicini, Anton Robert, Ivano Tavernelli, and Stefan Woerner. 2020. "Improving the Quantum Approximate Optimization Algorithm for the Knapsack Problem." *Physical Review A* 102 (3): 032415.

[8] Preskill, John. 2018. "Quantum Computing in the NISQ Era and Beyond." *Quantum* 2: 79.

[9] Kim, Youngseok, et al. 2023. "Evidence for the Utility of Quantum Computing Before Fault Tolerance." *Nature* 618: 500–505.

[10] Bravyi, Sergey, Andrew W. Cross, Jay M. Gambetta, Dmitri Maslov, Patrick Rall, and Theodore J. Yoder. 2024. "High-Threshold and Low-Overhead Fault-Tolerant Quantum Memory." *Nature* 627: 778–82.

## **Submission Details and Challenges**

The final submission for this hackathon is a 5-10 minute video presentation in any chosen format and your team's GitHub Repository. A Google Form for submission [can be found by clicking here](https://docs.google.com/forms/d/e/1FAIpQLSffK6jWlW7L8uXGhQ_336lzX1qnckdqiC-M593KWLag3hKDBw/viewform?usp=dialog). Only ONE team member has to submit, please do not duplicate submissions!

---

## 🏆 Winners 🏆

Congratulations to all winners and thank you everyone who competed!

<h2> 🥇 1st Place </h2>

**Coming Soon**
- [Repo Link]()
- Members:
  - 

<h2>🥈 2nd Place </h2>

**Coming Soon**
- [Repo Link]()
- Members:
  - 

<h2>🥉 3rd Place </h2>

**Coming Soon**
- [Repo Link]()
- Members:
  - 
 
 <h2>🏅 4th Place </h2>

**Coming Soon**
- [Repo Link]()
- Members:
  - 

---


## Certificates and Awards


- Winners will receive a digital certificate and a first place prize in the form of an interview with WISER for a fully paid fellowship is available. All participants will also receive general certificates and access to WISER's general summer education program.


### Useful Resources

- [Qiskit Youtubes](https://www.youtube.com/Qiskit)
- [QEE Resource Folder](https://drive.google.com/drive/folders/1h8H3HqeEugLJRGnizbYnJ-sTYo3oBGBV?usp=share_link)
- [Qompute 2025 Panel Discussion](https://drive.google.com/drive/folders/1h8H3HqeEugLJRGnizbYnJ-sTYo3oBGBV?usp=share_link)
- [QEE Lecture Series](https://drive.google.com/drive/folders/1h8H3HqeEugLJRGnizbYnJ-sTYo3oBGBV?usp=share_link)

## Feedback

Your opinions matter and we take them seriously to improve QEE events! Please complete the end-of-event survery to tell us your experience about Qompute 2026 and if you would like to attennd more events like this in the future. **Survey will be added closer to the event.**

