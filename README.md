3.7.1. Constant-0

	from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
	from numpy import pi
	qreg_q = QuantumRegister(2, 'q')
	creg_c = ClassicalRegister(2, 'c')
	circuit = QuantumCircuit(qreg_q, creg_c)
	circuit.reset(qreg_q[0])
	circuit.reset(qreg_q[1])
	circuit.x(qreg_q[0])
	circuit.x(qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.h(qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.h(qreg_q[1])
	circuit.measure(qreg_q[0], creg_c[0])
	circuit.measure(qreg_q[1], creg_c[1])

3.7.2. Constant-1

	from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
	from numpy import pi
	qreg_q = QuantumRegister(2, 'q')
	creg_c = ClassicalRegister(2, 'c')
	circuit = QuantumCircuit(qreg_q, creg_c)
	circuit.reset(qreg_q[0])
	circuit.reset(qreg_q[1])
	circuit.x(qreg_q[0])
	circuit.x(qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.h(qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.x(qreg_q[1])
	circuit.h(qreg_q[1])
	circuit.measure(qreg_q[0], creg_c[0])
	circuit.measure(qreg_q[1], creg_c[1])

3.7.3. Identity

	from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
	from numpy import pi
	qreg_q = QuantumRegister(2, 'q')
	creg_c = ClassicalRegister(2, 'c')
	circuit = QuantumCircuit(qreg_q, creg_c)
	circuit.reset(qreg_q[0])
	circuit.reset(qreg_q[1])
	circuit.x(qreg_q[0])
	circuit.x(qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.h(qreg_q[1])
	circuit.cx(qreg_q[0], qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.h(qreg_q[1])
	circuit.measure(qreg_q[0], creg_c[0])
	circuit.measure(qreg_q[1], creg_c[1])


3.7.4. Negation

	from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
	from numpy import pi
	qreg_q = QuantumRegister(2, 'q')
	creg_c = ClassicalRegister(2, 'c')
	circuit = QuantumCircuit(qreg_q, creg_c)
	circuit.reset(qreg_q[0])
	circuit.reset(qreg_q[1])
	circuit.x(qreg_q[0])
	circuit.x(qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.h(qreg_q[1])
	circuit.cx(qreg_q[0], qreg_q[1])
	circuit.h(qreg_q[0])
	circuit.x(qreg_q[1])
	circuit.h(qreg_q[1])
	circuit.measure(qreg_q[0], creg_c[0])
	circuit.measure(qreg_q[1], creg_c[1])
