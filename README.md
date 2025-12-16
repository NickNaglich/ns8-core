# NS8 Core

NS8 Core is a deterministic generator for structured synthetic 2D/3D fields.
It is designed as a controllable data source for machine learning experiments,
benchmarking, and visualization.

## What It Generates
- Discrete 2D and 3D lattice fields
- Periodic (toroidal) boundary conditions
- Deterministic, parameterized structure
- Repeatable outputs for benchmarking

## Why This Exists
Many ML benchmarks rely on random or unstructured data.
NS8 Core provides **structured synthetic fields** with known generative rules,
useful for:
- testing generalization
- studying symmetry learning
- evaluating temporal prediction
- debugging models on non-random data

## Quick Start
```python
from ns8.generator import generate_field

field = generate_field(N=32, k=1)
