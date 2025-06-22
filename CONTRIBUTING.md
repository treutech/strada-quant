# Contributing to Strada-Quant

First of all, thank you for your interest in contributing to **Strada-Quant**, an open computational finance platform developed by [Treu Technologies](https://github.com/treutech) and led by Raúl Estrada.

Strada-Quant is a modular system built in **Rust**, **CUDA**, and **Python**, with the goal of enabling high-performance, GPU-accelerated quantitative computing for research, education, and applied finance.

---

## Project Structure

```
strada-quant/
├── core/          ← Rust/CUDA logic (AGPL-3.0)
├── bindings/      ← Python bindings and CLI (MIT)
├── examples/      ← Usage and testing scripts
├── LICENSE
├── NOTICE
├── CONTRIBUTING.md
```

- The **core** is licensed under AGPL-3.0 to preserve openness.
- The **bindings** and tools are under MIT for wider adoption.

---

## Guiding Principles

We value:

- **Performance**: efficient computation on both CPU and GPU.
- **Reproducibility**: results that can be traced, tested, and audited.
- **Explainability**: code and algorithms should be understandable.
- **Collaboration**: we welcome contributors with diverse backgrounds.

---

## How to Contribute

### 1. Fork the Repository
Create your own fork via GitHub and clone it locally.

```bash
git clone https://github.com/YOUR_USERNAME/strada-quant
cd strada-quant
```

### 2. Set Up Your Environment
Install Rust and Python requirements:

```bash
# Rust toolchain
rustup install stable
rustup component add clippy rustfmt

# Python bindings
cd bindings
pip install -r requirements.txt
```

CUDA support is optional but recommended for full functionality.

### 3. Open or Pick an Issue
Check the [Issues tab](https://github.com/treutech/strada-quant/issues) or propose your own by opening a new one. Please include:

- A clear title and description
- Expected behavior and rationale
- Steps to reproduce (if reporting a bug)

### 4. Create a Feature Branch

```bash
git checkout -b feature/your-description
```

### 5. Code Style

- **Rust**: Run `cargo fmt` and `cargo clippy` before committing.
- **Python**: Use `black`, `flake8`, and `mypy` for consistency.

### 6. Commit and Push

```bash
git commit -m "Short, clear summary"
git push origin feature/your-description
```

### 7. Submit a Pull Request (PR)

Go to your fork and open a PR. Please:

- Reference related issues
- Describe what you changed and why
- Indicate whether your PR is ready or a draft

---

## Good First Issues

If you’re new to the project, look for [issues labeled good first issue](https://github.com/treutech/strada-quant/labels/good%20first%20issue).

We’re especially open to contributions in:

- Test coverage (unit and integration tests)
- Documentation and examples
- Performance benchmarking
- Implementing financial models (pricing, VaR, optimization)
- Improving GPU/CPU fallback logic

---

## License Notice

By contributing to this project, you agree that your contributions may be redistributed under the project's dual licensing model (AGPL-3.0 and MIT). Contributions will be attributed to their authors in the `NOTICE` file.

---

## Contact

For questions or guidance, feel free to open a [Discussion](https://github.com/treutech/strada-quant/discussions) or reach out via Issues.

Thank you for helping us build the future of open quantitative finance.
