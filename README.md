# Browser ML Projects

A collection of browser-based machine learning applications demonstrating real-time inference using ONNX Runtime Web and WebLLM.  
All projects run entirely client-side without server dependencies, ensuring privacy-preserving AI by processing data directly in the user's browser.  
Built with Next.js and modern web technologies, these applications showcase how powerful ML models can deliver interactive experiences through hardware-accelerated inference.

## Projects

### [ONNX Keyword Extracter](https://github.com/JadenKim-dev/onnx_keyword_extracter)

Combines PyTorch model conversion with real-time keyword extraction using a fine-tuned DistilBERT model (ml6team/keyphrase-extraction) converted to ONNX format. Takes raw text as input and automatically identifies and extracts key phrases.

### [ONNX Object Detection](https://github.com/JadenKim-dev/onnx_object_detection)

Real-time webcam-based object detection using YOLOv11 models converted to ONNX format. Combines a Python pipeline for model export with an interactive frontend. Features three model variants (Nano/2.6M, Small/9.4M, Medium/20.1M parameters) optimized for different speed-accuracy tradeoffs, with inference automatically selecting between WebGPU, WASM with SIMD, or fallback CPU execution.

### [Chrome WebLLM Chat](https://github.com/JadenKim-dev/chrome_webllm_chat)

Conversational AI chat application running the Llama-3-8B-Instruct model (4-bit quantized) using WebLLM and WebGPU acceleration. Features streaming token generation for responsive interactions, WebGPU compatibility detection (Chrome 113+, Edge 113+), and singleton pattern for efficient model management. Includes comprehensive test coverage using Vitest.
