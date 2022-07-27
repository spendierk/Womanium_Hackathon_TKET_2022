# Quantinuum's TKET challenge for the Womanium Global Hackathon

On behalf of Quantinuum, welcome to the Womanium Global Hackathon! This little guide should get you started quickly in `pytket`, a high-performance Python library for building and simplifying quantum programs.

TKET is the leading open-source developer toolkit designed to compile and optimize quantum programs. It is platform agnostic allowing it to target the world’s leading quantum hardware and simulators. It also enhances the performance of every Quantinuum product, including cybersecurity key-generation platform Quantum Origin, quantum computational chemistry and materials science package InQuanto, and lambeq, Quantinuum's quantum natural language processing and computational linguistics toolkit. 

If any questions arise during the hackathon, don't hesitate to contact me:
Kathrin Spendier: [kathrin.spendier@quantinuum.com](mailto:kathrin.spendier@quantinuum.com)

The content of this hackathon manual is as follows:
1) [Getting ready with `pytket`](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Getting%20ready%20with%20pytket.ipynb)
2) [Building circuits with `pytket`](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Building%20circuits%20with%20pytket.ipynb)
3) [Running a circuit on IBM's backends](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Running%20a%20circuit%20on%20IBM's%20backends.ipynb)
4) [Access to Quantinuum and IonQ Backends](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/Access%20to%20Quantinuum%20and%20IonQ%20Backends.ipynb)

This was a first glimpse of the workflow from the design of a quantum circuit to its execution. There is much more to discover by looking at an entire series of example notebooks for `pytket`
available on the [pytket github](https://github.com/CQCL/pytket/tree/master/examples).

Recommended examples applicable to this Hackathon you can go through as a continuation of this introduction include:
- [Run a circuit on the backends](https://github.com/CQCL/pytket/blob/master/examples/backends_example.ipynb)
- [Circuit Optimization](https://github.com/CQCL/pytket/blob/master/examples/compilation_example.ipynb)
- [Advanced techniques for creating circuits](https://github.com/CQCL/pytket/blob/master/examples/circuit_generation_example.ipynb)


# Your Hackathon Challenge: World-class Quantum chemistry with TKET

Your company builds hydrogen fuel cell vehicles and is interested in finding new ways for a cost-effective and compact hydrogen storage system. You are working in the research and development (R&D) department and are tasked to evaluate the feasibility to simulate the quantum state of a Lithium Hydride (LiH) molecule using a gate-based quantum device. Based on the known gate sets and the qubit coupling maps, you are tasked to find the best quantum device currently available.

## See [here](https://github.com/spendierk/Womanium_Hackathon_TKET_2022/blob/main/2022%20Womanium%20Hackathon%20challenge%20-%20Quantinuum.pdf) for challenge details


## Note
File "LiHJordanWignerMapper.qasm":
Ansatz LiH circuit in the form of a QASM code obtained by using the simplest qubit mapper/converter called the Jordan-Wigner Mapper.
