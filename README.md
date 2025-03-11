# Quantum-Computing-single-two-qubit-entanglements
The quantum bit, or qubit, which is the quantum equivalent of classical bits, is at the core
of quantum computing. Qubits have special characteristics like superposition and entanglement that
make quantum computers capable of solving some problems tenfold quicker than classical
computers. Qubit characteristics and application in quantum computation. We examine the ideas of
superposition, in which qubits can exist in several states at once, and entanglement, in which the
states of two qubits are interdependent even though they are separated by great distances.

Introduction
Qubits can exist in a superposition of states, whereas classical bits can only be in one of two states at
once, 0 or 1. This means that, according to the unusual laws of quantum mechanics, a qubit can
represent both 0 and 1 at the same time. Due to the extreme sensitivity of qubits to their
surroundings, the phenomenon of "decoherence," where quantum information is lost as a result of
interactions with outside causes, occurs.

Question 1)
The superposition state | is produced when the Hadamard gate is applied to the initial state |0]. The
qubit is in the state |ψ⟩ = (|0⟩ + |1⟩) / √2, after the H gate has been applied, meaning it has a 50%
chance of being measured as |0 and a 50% chance of being measured as |1. The classic illustration of
a quantum superposition is this one.
The superposition state | is produced when the Y gate is applied to the initial state |0⟩. The state is
changed as follows by the Y gate: |ψ⟩ = (|0⟩ - i|1⟩) / √2. 'i' stands for the imaginary unit, and the
phase difference between |0⟩ and |1⟩ defines this superposition state.
The superposition state | is produced when the Z gate is applied to the initial state |0⟩. The Z gate in
this instance, however, has no effect on the amplitudes or probabilities related to |0⟩ and |1⟩.
Although a phase shift of π is introduced, the state remains |ψ⟩ = |0⟩. It may not appear to be a
superposition in the conventional sense, but it is a real quantum state in which the probability
distribution of the qubit is unaltered
These three circuits use Hadamard (H), Y, and Z gates to show different superposition states. With
the same probability distribution, the H gate produces an equal superposition, the Y gate adds a
phase difference, and the Z gate applies a phase shift. The various superposition effects that can be
accomplished in quantum circuits are demonstrated by these actions.

Question 2)
A. |Φ+⟩ = 1/√2 (|00⟩ + |11⟩)
B. |Φ-⟩ = 1/√2 (|00⟩ - |11⟩)
C. |Ψ+⟩ = 1/√2 (|01⟩ + |10⟩)
D. |Ψ-⟩ = 1/√2 (|01⟩ - |10⟩)
Both qubits are initially in the state |0⟩ in each circuit. To produce the desired Bell states, the circuits
combine Hadamard gates (H), Pauli-X gates (X), and controlled-X gates (CX). To verify that the desired
Bell states have been properly generated, we will visualize the state vectors on the Bloch sphere after
the circuits have been run and examine the results of the measurements.
The four independent quantum circuits, each starting with both qubits in the state |0⟩, have been
created and implemented in Qiskit to show how Bell states A, B, C, and D can be created. The
visualizations of the state vectors and measurement results will demonstrate the fascinating and
fundamental nature of quantum processes in quantum computing and will demonstrate the
presence of quantum entanglement.

Question 3)
Quantum computing is renowned for its ability to carry out intricate computations and resolve issues
that are virtually insurmountable for conventional computers. The design and construction of a
challenging quantum circuit with at least three qubits and a variety of gates are shown in this
research. Exploring the complex and rich behavior that can be produced by quantum computation is
the goal.
Hadamard Gate (H): The initial qubit (qubit 0) is subjected to a Hadamard gate. By placing the qubit
in superposition, this gate ensures that there is an equal chance of measuring both |0| and |1|.
First and second qubits (qubits 0 and 1) are entangled using a controlled-NOT gate (CNOT gate, CX).
The two qubits are quantum-correlated as a result of this entanglement.
Z Gate (Z): The third qubit (qubit 2) is subjected to a Z gate. Phase flips, which are essential quantum
operations, are introduced by this gate.
Decoherence is the loss of quantum coherence as a result of environmental interactions. We apply
depolarizing errors to gates and relaxation errors to qubits in this simulation. The noise model
consists of Gate-level noise is introduced by depolarizing errors. To replicate the effects of faulty gate
operations, a depolarizing error of 0.1 is used.
The statevector simulator in Qiskit is used to run the transpile circuit. After applying the gates and
taking into consideration the added noise, the resultant statevector is a representation of the
quantum state. The entanglement and intricate structure of the quantum state are revealed through
the visualization of the statevector on a Bloch sphere.
The advanced quantum circuit on display demonstrates the flexibility and strength of quantum
computing. The complex quantum processes that can be tapped into for quantum information
processing are demonstrated through the use of gates, entanglement, and noise simulation. For
quantum computing to reach its full potential in tackling practical issues, it is crucial to comprehend
and grasp such complexity.
Challenges Faced
Gate selection: Choosing the proper gates and figuring out their order might be difficult. Selecting
the appropriate combination of gates is essential for achieving the desired quantum state or
behavior since different gates have different effects on qubits. Designing gates that produce and
manipulate the entanglement between qubits can be difficult. In order for quantum computing to
function effectively, entanglement must be properly formed.
Design rationale for circuit
Design Justification: The |+ Bell state is a maximally entangled state in which both qubits are coupled
and in a superposition of the |0 and |1 states. To achieve this condition:
The initial qubit (qubit 0) is given a Hadamard gate (H). The first qubit is placed in a superposition of
|0| and |1| by this gate.
With the first qubit acting as the control and the second qubit serving as the target, we apply a CNOT gate(CX). Two qubits are entangled by this gate, putting them in correlated state.
