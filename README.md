# Unsafe Rust Pointer Modification Example

This repository demonstrates a common error when working with raw pointers in Rust: modifying a vector's contents via a raw pointer after the vector's internal structure has been changed.  This can lead to undefined behavior, including crashes or data corruption.

The `bug.rs` file shows the erroneous code. The `bugSolution.rs` provides a safer alternative using proper Rust techniques to avoid the issue.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Compile and run `bug.rs` using `rustc bug.rs && ./bug`. Observe the potential unpredictable behavior or crashes.
4. Compile and run `bugSolution.rs` using `rustc bugSolution.rs && ./bugSolution`. Observe the correct and safe behavior. 

## Contributing

Contributions are welcome. Please open an issue or submit a pull request to improve the example or add more scenarios.  