# Browser ML Projects

A collection of browser-based machine learning applications demonstrating real-time inference using **ONNX Runtime Web** and **WebLLM**.

## Overview

All projects run entirely **client-side** without server dependencies, ensuring privacy-preserving AI by processing data directly in the user's browser. Built with **Next.js** and modern web technologies, these applications showcase how powerful ML models can deliver interactive experiences through hardware-accelerated inference.

---

## Projects

### [ONNX Keyword Extracter](https://github.com/JadenKim-dev/onnx_keyword_extracter)

Real-time keyword extraction using a fine-tuned DistilBERT model converted to ONNX format.

**Features:**
- PyTorch model conversion pipeline
- Fine-tuned DistilBERT model (ml6team/keyphrase-extraction)
- Automatic key phrase identification from raw text
- ONNX Runtime Web inference

---

### [ONNX Object Detection](https://github.com/JadenKim-dev/onnx_object_detection)

Real-time webcam-based object detection using YOLOv11 models.

**Features:**
- Python pipeline for ONNX model export
- Interactive frontend with live webcam feed
- Multiple model variants for different use cases:
  - **Nano**: 2.6M parameters (fastest)
  - **Small**: 9.4M parameters (balanced)
  - **Medium**: 20.1M parameters (most accurate)
- Automatic runtime selection: WebGPU → WASM with SIMD → CPU fallback

---

### [Chrome WebLLM Chat](https://github.com/JadenKim-dev/chrome_webllm_chat)

Conversational AI chat application running entirely in the browser.

**Features:**
- Llama-3-8B-Instruct model (4-bit quantized)
- WebLLM and WebGPU acceleration
- Streaming token generation for responsive interactions
- WebGPU compatibility detection (Chrome 113+, Edge 113+)
- Singleton pattern for efficient model management
- Comprehensive test coverage using Vitest

---

## Technology Stack

- **Frontend**: Next.js, React
- **ML Runtimes**: ONNX Runtime Web, WebLLM
- **Acceleration**: WebGPU, WebAssembly (SIMD)
- **Models**: DistilBERT, YOLOv11, Llama-3
- **Testing**: Vitest, Pytest
