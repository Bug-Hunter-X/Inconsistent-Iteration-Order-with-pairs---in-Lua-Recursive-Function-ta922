# Inconsistent Iteration Order with pairs() in Lua Recursive Function

This repository demonstrates a potential issue with Lua's `pairs` iterator when dealing with recursive table traversal.  The function `foo` recursively iterates over a table, but the order of iteration using `pairs` isn't guaranteed to be consistent across different Lua implementations or even different runs of the same code. This can lead to unexpected results if the processing order is important in the recursive logic.

The `bug.lua` file contains the problematic code, while `bugSolution.lua` provides a solution using a sorted iteration technique to ensure a predictable order.

## Solution:
The solution involves using a custom iteration approach or a library function that guarantees a specific ordering.