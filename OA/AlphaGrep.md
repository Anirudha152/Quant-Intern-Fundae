# AlphaGrep Online Assessment Problems


## 1. Connected Graph Distance Calculation

### Problem Statement

Consider a connected graph consisting of nodes and bidirectional edges. Each edge is 1 unit of distance long, and only one edge connects any two nodes. There is one cycle in the graph. For each node, determine its shortest distance from the cycle and return the distances in an integer array. If a node is in the cycle, its distance is 0.

#### Example

- `g_nodes = 6`
- `g_edges = 6`
- `g_from = [1, 2, 1, 3, 1,2]`
- `g_to =   [2, 3, 3, 5 ,4, 6]`

The cycle contains nodes 1, 2, and 3 with distance 0. Nodes 4, 5, and 6 are each 1 unit distance from the cycle.

### Function Signature (C++)
```cpp
vector nodeDistance(int g_nodes, vector g_from, vector g_to);
```

## 2. Divisible Range

### Problem Statement

Given an integer array `arr` with `n` elements, and two integers `k` and `x`, find the number of pairs of indices `(i, j)` where `0 ≤ i  arr, int k, int x);
```

#### Constraints

- `2 ≤ n ≤ 10^5`
- `1 ≤ k, x ≤ 10^9`
- `1 ≤ arr[i] ≤ 10^9`

## 3. Process Execution

### Problem Statement

A cloud services platform added `n` new processors, each with a computing power specified by `power[i]`. Not all processors can be utilized simultaneously. If a processor with computing power `power[i]` is in use, then processors with computing power `power[i] + 1` or `power[i] - 1` cannot be used. Additionally, each processor can only be used once.

Determine the maximum possible sum of the computing powers of the selected processors.

#### Example

- `n = 7`
- `power = [3, 3, 3, 4,[4][1]`

One optimal way (0-based indexing):

- Choose processor 6 (`power = 8`)
- Choose processor 5 (`power = 1`)
- Choose processor 0/1/2 (`power = 3`)

The sum is 8 + 1 + 3 + 3 + 3 = 18.

### Function Signature (C++)
```cpp
long getMaximumPower(vector power);
```

## 4. Cost-Efficient Task Cleanup

### Problem Statement

You are given an array `taskCosts` of size `n`, where each element represents the cost of executing a task.

- For each task, you can either retain it (paying its individual cost) or remove it using a cleanup operation.
- Cleanup operations are available in bundles, each providing `operationsPerBundle` cleanup operations at a cost of `bundleCost` per bundle.
- Multiple bundles can be allocated.
- Unused operations within a bundle are allowed.

Compute the minimum total cost: sum of execution costs of all retained tasks plus total cost of allocated cleanup bundles.

### Function Signature (C++)
```cpp
long getMinimumCost(vector taskCosts, int operationsPerBundle, int bundleCost);
```

#### Constraints

- `taskCosts[]`: array representing the cost of each task
- `operationsPerBundle`: number of cleanup operations available in one bundle
- `bundleCost`: cost per cleanup bundle
