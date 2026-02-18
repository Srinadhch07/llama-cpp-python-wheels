# llama-cpp-python Community Wheels

Unofficial **precompiled Windows wheels** for `llama-cpp-python`, built to support **early Python versions** where official binaries may not yet be available.

These wheels allow developers to install `llama-cpp-python` instantly without requiring Visual Studio C++ Build Tools or local compilation.

---

## Available Wheels

| Package Version | Python | Platform | Download |
|----------------|--------|----------|----------|
| 0.3.16 | 3.14 | Windows x64 | See Releases |

More Python versions will be added as they become available.

---

## Installation

Download the appropriate `.whl` file from the **Releases** page and install using:

```bash
pip install llama_cpp_python-<version>-cpXXX-win_amd64.whl
```

Example:

```bash
pip install llama_cpp_python-0.3.16-cp314-cp314-win_amd64.whl
```

---

## Usage Example

```python
from llama_cpp import Llama

llm = Llama(model_path="model.gguf")
response = llm("Explain attention mechanism in simple words.", max_tokens=100)
print(response["choices"][0]["text"])
```

---

## Notes

- These wheels contain **only the Python bindings**. Model files (GGUF) must be downloaded separately from Hugging Face or other sources.
- Builds are intended as **community early-release binaries** until official upstream wheels are published.
- Compatible only with the specified **Python version and platform**.

---

## License

`llama-cpp-python` and `llama.cpp` are distributed under the **MIT License**. Please refer to the upstream repositories for full license details.

---

## Contributing

Contributions are welcome. If you build wheels for additional Python versions or platforms, feel free to open a pull request or submit a release.

