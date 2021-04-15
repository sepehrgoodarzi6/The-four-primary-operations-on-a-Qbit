3.7.1. Constant-0
The source code of the designed circuit is available at:
By measuring the results of the Qbits, we got the results showing on plots a 3D-sphere. According to the probability states and also amplitude, the measured probability of states of Qbits is a hundred percent |11⟩  (which we have demonstrated in pervious section).
 
Figure 6. The implemented circuit for Constant-0 test

 
Figure 7. The prediction of the probability states of Qbits of Constant-0 test
 
Figure 8. The amplitude on computational basis states of Constant-0 test

 
Figure 9. 2D version of the 3D-sphere of Constant-0 test

Source Code of Constant-0 test:
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
The source code of the designed circuit is available at:
According to the probability states and also amplitude, the measured probability of states of Qbits is a hundred percent |11⟩, exactly the same as the results we got from testing Constant-0.

 
Figure 11. The implemented circuit for Constant-1 test

 
Figure 12. The prediction of the probability states of Qbits of Constant-1 test
 
Figure 13. The amplitude on computational basis states of Constant-1 test

 
Figure 14. 2D version of the 3D-sphere of Constant-1 test

Source Code of Constant-0 test:
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
The source code of the designed circuit is available at:
According to the probability states and also amplitude, the measured probability of states of Qbits is a hundred percent |10⟩, which varies from the results of the Constants.



 
Figure 15. The implemented circuit for Identity test

 
Figure 16. The prediction of the probability states of Qbits of Identity test

 
Figure 17. The amplitude on computational basis states of Identity test

 
Figure 18. 2D version of the 3D-sphere of Identity test

Source Code of Identity test:
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
The source code of the designed circuit is available at:
According to the probability states and also amplitude, the measured probability of states of Qbits is a hundred percent |10⟩, which varies from the results of the Constants and is the same as Identity.

 
Figure 19. The implemented circuit for Negation test

 
Figure 20. The prediction of the probability states of Qbits of Negation test

 
Figure 21. The amplitude on computational basis states of Negation test

 
Figure 22. 2D version of the 3D-sphere of Negation test

Source Code of Negation test:
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

