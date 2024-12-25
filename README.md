# Lua Recursive Table Traversal Bug

This repository demonstrates a common error in Lua involving unpredictable iteration order when recursively traversing tables using `pairs`.  The `pairs` iterator does not guarantee any specific order of iteration, which can lead to unexpected results in recursive functions.

The `bug.lua` file contains the problematic code, while `bugSolution.lua` provides a corrected version.

## Bug

The main issue is that the order of processing nested tables is not defined, potentially leading to incorrect results if the processing depends on a specific order.