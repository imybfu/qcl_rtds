# 01qiskit_primary

```python
pip install qiskit
pip install qiskit[visualization]
```

基本指令
1. circuit
```python
from qiskit import QuantumCircuit
QuantumCircuit(2, 2)
h(0)
cx(0, 1)
measure([0,1], [0,1])
```
2. simulator
```python
from qiskit import Aer
Aer.get_backend('qasm_simulator')
```
3. IBMQ
```python
from qiskit import IBMQ
IBMQ.save_account('token')
IBMQ.load_account()
```
4. provider
```python
IBMQ.get_provider('ibm-q')
```
5. backend
```python
provider.get_backend('ibmq_lima')
```
6. job
```python
execute(circuit,backend=simul,shots=1000)
from qiskit.tools.monitor import job_monitor
job_monitor(job2)
```
7. result
```python
job1.result()
```
8. count
```python
result1.get_counts()
```
9. plot
```python
from qiskit.visualization import plot_histogram
plot_histogram(result1.get_counts())
```
