# Quantinuum's TKET challenge for the Womanium Global Quantum Hackathon

On behalf of [Quantinuum](https://www.quantinuum.com/), welcome to the Womanium Global Quantum Hackathon! This little guide should get you started quickly in `pytket`, a high-performance Python library for building and simplifying quantum programs.

[TKET](https://www.quantinuum.com/developers/tket) is the leading open-source developer toolkit designed to compile and optimize quantum programs. It is platform agnostic allowing it to target the world’s leading quantum hardware and simulators. It also enhances the performance of every Quantinuum product, including cybersecurity key-generation platform Quantum Origin, quantum computational chemistry and materials science package InQuanto, and lambeq, Quantinuum's quantum natural language processing and computational linguistics toolkit. 

If any questions arise during the hackathon, don't hesitate to contact me:
Kathrin Spendier: [kathrin.spendier@quantinuum.com](mailto:kathrin.spendier@quantinuum.com)

The content of this hackathon manual is as follows:
1) [Getting ready with `pytket`](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Getting%20ready%20with%20pytket.ipynb)
2) [Building circuits with `pytket`](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Building%20circuits%20with%20pytket.ipynb)
3) [Why TKET?](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Why%20TKET.ipynb)
4) [Running a circuit on IBM's backends](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Running%20a%20circuit%20on%20IBM's%20backends.ipynb)
5) [Access to Quantinuum and IonQ Backends](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Access%20to%20Quantinuum%20and%20IonQ%20Backends.ipynb)

This was a first glimpse of the workflow from the design of a quantum circuit to its execution. There is much more to discover by looking at an entire series of example notebooks for `pytket`
available on the [pytket github](https://github.com/CQCL/pytket/tree/master/examples).

Recommended TKET examples applicable to this Hackathon you can go through as a continuation of this introduction include:
- [Run a circuit on the backends](https://github.com/CQCL/pytket/blob/master/examples/backends_example.ipynb)
- [Circuit Optimization](https://github.com/CQCL/pytket/blob/master/examples/compilation_example.ipynb)
- [Advanced techniques for creating circuits](https://github.com/CQCL/pytket/blob/master/examples/circuit_generation_example.ipynb)


# Your Hackathon Challenge: World-class Quantum chemistry with TKET

Your company builds hydrogen fuel cell vehicles and is interested in finding new ways for a cost-effective and compact hydrogen storage system. You are working in the research and development (R&D) department and are tasked to evaluate the feasibility to simulate the quantum state of a Lithium Hydride (LiH) molecule using a gate-based quantum device. Based on the known gate sets and the qubit coupling maps, you are tasked to find the best quantum device currently available.

## Beginner: 
You will first get a feel for how TKET optimizes and compiles sample circuits for a given backend. You can create a sample circuit of your choice, or you can use some circuits, given as QASM code, [here](https://github.com/spendierk/ethz-hackathon22/tree/main/benchmarking/circuits). Then optimize and run this sample circuit on different backends. Here is a list of questions to get you started:
1)	Which gate-based quantum computers are accessible to you to implement your circuit?
2)	Which circuit parameters should be minimized for the most efficient circuit implementation for a given backend?
3)	What are the main features of TKET, and how can you apply them here?
4)	Which backend is the best for a given sample circuit and why?

## Knowledgeable: 
Instead of using a sample circuit, you will perform the tasks outlined for Beginner above for an actual LiH circuit. A given ansatz LiH circuit in the form of a QASM file (LiHJordanWignerMapper.qasm) will be supplied to you for your analysis [here](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/LiHJordanWignerMapper.qasm). The circuit was obtained by using the simplest qubit mapper/converter called the Jordan-Wigner Mapper. This circuit is quite deep. Before optimization, the circuit will have a total of 12 qubits and more than 16,000 gates.

## Advanced: 
You are comfortable with how TKET can optimally route circuits onto real hardware. You are now asked to use the VQE algorithm to estimate the ground state energy for a LiH molecule. You should create your own ansatz LiH circuit for this challenge. Is it possible to create a 6-qubit ansatz circuit with a different mapper/converter than the Jordan-Wigner Mapper? Do you get different results depending on the quantum computer/simulator used? How do your results compare to known values? Are there any limitations you are confronted with? You can consult the [Qiskit nature documentation](https://qiskit.org/documentation/nature/tutorials/index.html) to get you started.

Problem expansion for Advanced: You are also considering how errors for different operations affect your analysis, i.e. mapping should be noise-aware. Can you implement some error mitigation techniques to improve your results?

## See [here](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/2022%20Womanium%20Hackathon%20challenge%20-%20Quantinuum.pdf) for challenge details

## Note
File "LiHJordanWignerMapper.qasm" located in this GitHub repository is the the ansatz LiH circuit in the form of a QASM code obtained by using the simplest qubit mapper/converter called the Jordan-Wigner Mapper.
