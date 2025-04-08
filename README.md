# 🔁 push_swap

## 🧠 What is this?

`push_swap` is a sorting algorithm visualizer built with C as part of the 42 curriculum.  
The task is to sort a stack of integers using **only a limited set of stack operations**, with the **least possible moves**.

This project is all about:
- Data structures (linked lists for stacks)
- Sorting algorithms
- Writing efficient and clean code under tight constraints

## 🚀 How it works

The program uses two stacks (`a` and `b`) and simulates sorting using operations like `push`, `swap`, `rotate`, and `reverse rotate`.  
It outputs the list of instructions that would sort the input.

For small datasets, I implemented specific sorting strategies.  
For larger ones, the project uses a binary radix sort for efficiency.

## ⚙️ Usage

Build the project:
```bash
make
Run the program with a list of integers:

bash
Copy
Edit
./push_swap 3 2 1
You can pipe the result into the checker (bonus part) to verify correctness:

bash
Copy
Edit
ARG="3 2 1"
./push_swap $ARG | ./checker $ARG
💡 Allowed Operations
sa, sb, ss — swap the first two elements

pa, pb — push the top element to the other stack

ra, rb, rr — rotate stack up

rra, rrb, rrr — rotate stack down

📁 Structure
bash
Copy
Edit
push_swap/
├── src/         # Sorting logic, utils, stack ops
├── checker/     # Bonus: validate the operations
├── includes/    # Header files
├── Makefile
└── README.md
🧪 Features
Input parsing with error/overflow check

Duplicate detection

Adaptive sorting logic

Modular, readable code
