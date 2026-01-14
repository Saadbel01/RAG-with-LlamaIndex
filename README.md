# Simple RAG with LlamaIndex and Hugging Face

This project is a simple and instructive Retrieval-Augmented Generation (RAG) example.

You can:
- load your own document (or a folder of documents),
- choose the LLM you want,
- choose generation token settings,
- ask questions and see retrieved evidence chunks.

## Project File

- `build_rag_with_llama2_and_llamaindex.ipynb`

## What This Notebook Teaches

The notebook is organized in clear steps:
1. Install dependencies
2. Import libraries
3. Enter user settings (document path, model, tokens)
4. Optional Hugging Face token setup
5. Load document(s)
6. Create LLM + embedding model
7. Configure chunking settings
8. Build vector index
9. Ask question and inspect retrieved chunks

This helps you understand not only the final answer, but also the retrieval step of RAG.

## Requirements

- Python environment with Jupyter support
- Internet access for model/package download
- Optional: CUDA GPU (faster)
- Optional: Hugging Face token for gated models

## Quick Run

1. Open the notebook.
2. Run all cells from top to bottom.
3. At Step 2, enter:
   - document path,
   - model choice,
   - max tokens,
   - temperature,
   - retriever top_k,
   - optional HF token.
4. Ask your own question in the final cells.

## Good Practices Used

- `%pip` is used inside notebook cells.
- Input path is validated before loading documents.
- Public and gated model usage is supported.
- Retrieval evidence is printed for transparency.
- Chunk size and overlap are explicitly configured.

## Tips

- If imports are unresolved, run the install cell first, then rerun notebook cells.
- Start with a small model if your machine has limited memory.
- Use `temperature = 0.0` for factual and stable answers.
