## Generic module for SMT solver

### How to use

1. Clone this repository to your local env.

```
cd Desktop
git clone https://github.com/tomohiroyoshida/SMT.git
```

2. solve problem with SMT solver
   We would like to skip the explanation on how to set up Haskell environment here.
   We use GHC and Z3.
   If you want to solve [killer sudoku](https://en.wikipedia.org/wiki/Killer_sudoku) problem with [Z3](https://github.com/Z3Prover/z3), run the following commands:

```
cd SMT
runghc killer input.txt
z3 smt.smt2
```

Then you can get the answer of the killer sudoku problem like this:

```
sat
((x11 2)
(x12 1)
(x13 5)
(x14 6)
(x15 4)
(x16 7)
(x17 3)
(x18 9)
(x19 8)
(x21 3)
(x22 6)
(x23 8)
(x24 9)
(x25 5)
(x26 2)
(x27 1)
(x28 7)
(x29 4)
(x31 7)
(x32 9)
(x33 4)
(x34 3)
(x35 8)
(x36 1)
(x37 6)
(x38 5)
(x39 2)
(x41 5)
(x42 8)
(x43 6)
(x44 2)
(x45 7)
(x46 4)
(x47 9)
(x48 3)
(x49 1)
(x51 1)
(x52 4)
(x53 2)
(x54 5)
(x55 9)
(x56 3)
(x57 8)
(x58 6)
(x59 7)
(x61 9)
(x62 7)
(x63 3)
(x64 8)
(x65 1)
(x66 6)
(x67 4)
(x68 2)
(x69 5)
(x71 8)
(x72 2)
(x73 1)
(x74 7)
(x75 3)
(x76 9)
(x77 5)
(x78 4)
(x79 6)
(x81 6)
(x82 5)
(x83 9)
(x84 4)
(x85 2)
(x86 8)
(x87 7)
(x88 1)
(x89 3)
(x91 4)
(x92 3)
(x93 7)
(x94 1)
(x95 6)
(x96 5)
(x97 2)
(x98 8)
(x99 9))
```
