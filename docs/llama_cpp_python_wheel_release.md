# llama-cpp-python Windows Wheel (Python 3.14)

This release provides a **precompiled Windows wheel** for `llama-cpp-python` built using MSVC Build Tools for **Python 3.14 (win_amd64)**.

The wheel eliminates the need to install Visual Studio C++ Build Tools or compile from source, enabling fast and reliable installation for local LLM and RAG workflows.

---

## Build Details
- Package: `llama-cpp-python`
- Version: 0.3.16
- Python: 3.14
- Platform: Windows (64-bit)
- Compiler: MSVC v143 (Visual Studio Build Tools)
- Backend: CPU (llama.cpp)

---

## Installation

Download the wheel file from this release and install:

```bash
pip install llama_cpp_python-0.3.16-cp314-cp314-win_amd64.whl
```

No additional compilation or build tools are required.

---

## Usage Example

```python
from llama_cpp import Llama

llm = Llama(model_path="model.gguf")

output = llm("Explain transformers in simple terms.", max_tokens=100)
print(output["choices"][0]["text"])
```

---

## Notes
- This release contains **only the Python wheel**. Model files (GGUF) must be downloaded separately from Hugging Face or other providers.
- Built using official `llama.cpp` backend under the MIT License.
- Intended for developers running local LLM inference, RAG pipelines, and offline experimentation.

---

## License
`llama-cpp-python` and `llama.cpp` are distributed under the **MIT License**. Please refer to the upstream repositories for full license details.

