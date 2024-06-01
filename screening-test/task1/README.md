# QuantumAI.Cloud Screening Test

💡 Develop a Python program to generate a list of 2n unique random positive integers, each using a maximum of n bits and represented in decimals, and another random positive integer, k, using n bits.  Then, choose one (or more, if you prefer) of the following options to implement:

1. Check if k exists in the list.

2. Find all integers less than k in the list.

Display the results and the number of steps required to achieve them.

# Example

Below is a suggested structure and sample input/output, but feel free to be creative as long as you meet the key requirements.

```Python
def generate_random_list(n : int):
"""
n: positive integer value
Returns random number k and list_n of 2n unique positive integers.
"""

def search_k(k: int, list_n: list[int]):
"""
k: positive integer number
list_n: list of positive integers.
Returns (True, n_steps) if k exists, and (False, n_steps) otherwise,
where n_steps is the number of steps needed.
"""

def less_than_k(k: int, list_n: list[int]):
"""
k: positive integer number
list_n: list of positive integers.
Return (list_nk, n_steps), where list_nk contains all numbers in list_n that 
are less than k (if any), n_steps is the number of steps needed.
"""

# Example:
k, list_n = generate_random_list(3)
k_exist = search_k(k, list_n)
list_nk = less_than_k(k, list_n)
print(k, list_n)
print(k_exist)
print(list_nk)

# Output
5, [3, 2, 5, 1, 6, 7]
(True, 3)
([2, 1], 6)
```

Discussion and Bonus task

Write a brief discussion on the following points in your Jupyter Notebook (.ipynb) or Markdown (.md) file (both Vietnamese and English are acceptable and will not affect your outcome):

1. Discuss the method used for generating random numbers and its impact on the results. Can we generate the same random values multiple times? If so, please add that implementation.

2. Analyze the average number of trials needed to solve Task 1.a and 1.b. Try to find the optimal solution with the smallest number of steps required. Discuss the complexities involved in the operations.

3. Which problems in Task 1 can be improved using quantum computing? Why?

🔥 Bonus 1 (recommended): Propose a quantum solution for Task 1 and implement a quantum program using any quantum SDKs (such as Qiskit, Cirq, or Braket) to solve any parts of Task 1.

🔥 Bonus 2: Propose a simple deployment approach for this task by packaging your program in a Docker container and publishing these implementations as API services using any API frameworks (such as Flask and FastAPI). Implement your proposal if possible.