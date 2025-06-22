# Strada-Quant

**Strada-Quant** is an open-source, high-performance computational finance platform developed by [Treu Technologies](https://github.com/treutech) and led by Raúl Estrada.

It is designed for advanced financial modeling, backtesting, and simulation with a modular architecture written in **Rust**, accelerated by **CUDA**, and exposed via **Python bindings** for usability.

---

## Project Goals

- GPU-accelerated core computations using Rust + CUDA
- Transparent logic for backtesting, VaR, and combinatorial engines
- Python bindings via PyO3 for scripting and integration
- Automatic CPU/GPU fallback
- Modular crates for strategies, execution, analysis, and bindings

---

## Project Structure

```
strada-quant/
├── crates/              # Core Rust + CUDA modules (AGPL-3.0)
├── bindings/python/     # Python bindings via PyO3 (MIT)
├── examples/            # Usage examples and CLI tools
├── LICENSE              # Dual license: AGPL-3.0 (core), MIT (bindings/tools)
├── NOTICE               # Legal attributions and project credits
├── CONTRIBUTING.md      # How to contribute
├── Cargo.toml           # Workspace configuration
```

---

## Usage

> The project is in early development. Expect rapid changes and breaking updates.

Clone the repository:

```bash
git clone https://github.com/treutech/strada-quant
cd strada-quant
```

Build the Rust workspace:

```bash
cargo build --release
```

Install Python bindings (WIP):

```bash
cd bindings/python
pip install -e .
```

---

## Contributing

We welcome contributions! See [`CONTRIBUTING.md`](./CONTRIBUTING.md) to get started.

---

## License

- Core components: **AGPL-3.0**
- Bindings and tools: **MIT**

See [`LICENSE`](./LICENSE) and [`NOTICE`](./NOTICE) for details.

---

## Lead Developer

**Raul Estrada**  
[github.com/uurl](https://github.com/uurl)

---
Built with ❤️ by [Treu Technologies](https://github.com/treutech)
