# Project Philosophy

## Vision

Build a reusable DSP framework capable of processing IQ recordings from multiple sources.

Initially this project will support RTL-SDR.

Eventually the goal is to have it support other sources including

- HackRF
- BladeRF
- Recorded IQ files
- Simulated signals

---

## Development Philosophy

1. Use MATLAB to create prototypes
2. Use MATLAB to validate prototypes
3. Implement in C++
4. Create tests for C++
5. Document everything

---

## Coding Standards

- C++20
- CMake
- vcpkg
- MATLAB with various toolboxes including DSP and communications toolboxes

---

## Validation Strategy

Every DSP algorithm should have

- MATLAB implementation
- C++ implementation
- Comparison tests

No algorithm should exist only in C++

---

## Repository Organization

src/
- C++ source code
include/
- C++ libraries
tests/
- C++ test files
matlab/
- Any MATLAB files including helper functions and testing files
docs/
- Documentation for everything
data/
- Recordings including .iq and .wav files
