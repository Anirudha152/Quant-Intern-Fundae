

### 1. **Correlation Matrix Consistency**

> **Problem:**
> Given a 3×3 correlation matrix:

```
Σ = [  1    1/4   1/3  ]  
    [ 1/4    1     x  ]  
    [ 1/3    x     1  ]
```

Find the **difference between the maximum and minimum values** that `x` can take such that `Σ` remains a valid correlation matrix (i.e., symmetric and positive semi-definite).

> **Objective:**
> Return `x_max - x_min`, rounded to 3 decimal places.

---

### 2. **Voter Transition Markov Process**

> **Problem:**
> On a distant planet, voters support one of two political parties: A or B. Each voter votes in every election held every 4 years. After every election:

* An A supporter switches to B with probability 11%.
* A B supporter switches to A with probability 8%.

Initially, B wins 70% to 30%.
**Find the expected vote share of party B 10,000 years (i.e., 2500 elections) later.**

> **Objective:**
> Return the long-term expected percentage of B voters, to 2 decimal places.

---

### 3. **Optimal Mystery Box Strategy**

> **Problem:**
> You have 3 identical mystery boxes, each containing one unique figurine (A, B, C). You do not know which box contains which.

* You can sell an **unopened** box for **\$4**.
* If you **open** a box, you receive the **market value** of the figurine:

  * A: \$2
  * B: \$4
  * C: \$6

Your goal is to **maximize expected profit** by opening some boxes and deducing contents.

> **Objective:**
> Return the **maximum expected profit**, rounded to **2 decimal places**.

---

### 4. **Poisson Arrivals and Exponential Bus Times**

> **Problem:**

* Passengers arrive at a bus stop according to a **Poisson process** with rate **10 per unit time**.
* Buses arrive according to an **exponential distribution** with rate **4**, i.e., expected arrival time is `1/4` units.

> **Objective:**
> Compute the **expected number of passengers** on a bus, rounded to **1 decimal place**.

---

### 5. **Sum of Squares of Eigenvalues**

> **Problem:**
> Given the 3×3 matrix:

```
M = [3 0 1]
    [0 3 1]
    [1 1 2]
```

> **Objective:**
> Find the **sum of squares of its eigenvalues**, rounded to **1 decimal place**.

---

### 6. **Bayesian Inference on Biased Coin**

> **Problem:**
> You are given a coin that is biased with **2/3 probability** towards either **heads or tails**, with **equal 50-50 prior**.
> You flip the coin **5 times** and observe **2 heads**.

> **Objective:**
> What is the **posterior probability** that the coin is biased **towards heads**? Round to **2 decimal places**.



## 🧠 Concepts Tested

* Linear algebra: positive semi-definite matrices, eigenvalues
* Markov chains and transition matrices
* Bayesian probability
* Poisson and exponential distributions
* Expected value and optimization under uncertainty

