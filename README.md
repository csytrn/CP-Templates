# CP Templates

This is a compilation of templates that I use for competitive programming (CP) contests. It currently only has C++ templates.

## C++ (/cpp/)
| Template | File | Description | Dependencies |
| - | - | - | - |
| C++ Shortcut | .zshrc | Contains a simple "run" command that simplifies compiling and running C++ files: makes `run file` shorthand for `g++ -std=gnu++17 file.cpp -o file && ./file`. You must add the command to your local ~/.zshrc file for Zsh, ~/.bashrc for Bourne shell, etc. | |
| C++ Super Header | bits/stdc++.h | A "super header" file ([docs](https://gcc.gnu.org/onlinedocs/gcc-4.8.0/libstdc++/api/a01541_source.html)). This file should already exist in the C++ library, but sometimes doesn't. | |
| Base | base.cpp | Basic environment configuration, common typedefs, and helper functions; can be independently run as a full program. **Start every program from this.** | C++ Super Header (if not already in library) |
| DSU 1 | dsu1.cpp | Disjoint set union (DSU) with persistence and rollback. | Base |
| DSU 2 | dsu2.cpp | DSU with dynamic connectivity offline (DCO). | DSU 1 |
| Number Theory | nt.cpp | Common constants and a `mint` struct with mathematical operations for modular arithmetic | Base |
| Segment Tree 1 | st1.cpp | Basic segment tree data structure | Base |
| Segment Tree 2 | st2.cpp | Segment tree with methods to add to a single element and get the sum over a segment. Easy to generalize to many common applications. | Base |
| LCA | lca.cpp | Lowest common ancestor (LCA) with binary lifting | Base |