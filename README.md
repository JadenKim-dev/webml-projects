# ONNX Projects

A collection of browser-based machine learning applications demonstrating real-time inference using ONNX Runtime Web.

## Projects

### [ONNX Keyword Extracter](https://github.com/JadenKim-dev/onnx_keyword_extracter)

A full-stack browser-based keyword extraction system that combines PyTorch model conversion and real-time inference in web browsers. It takes raw text as input and automatically identifies and extracts key phrases using a fine-tuned DistilBERT model (ml6team/keyphrase-extraction) converted to ONNX format. The system enables client-side processing without server dependencies, providing privacy-preserving keyword extraction directly in the user's browser.

Built with Next.js 16, ONNX Runtime Web, and Transformers.js, the project features multi-backend execution support (WebGPU → WebGL → WASM fallback), intelligent BIO-tagged token classification, and advanced post-processing with confidence scoring and stopword removal. The application supports both FP32 (253MB) and INT8 (64MB) model variants.

### [ONNX Object Detection](https://github.com/JadenKim-dev/onnx_object_detection)

A browser-based real-time object detection application that leverages YOLOv11 deep learning models converted to ONNX format for efficient inference in web environments. The project combines a Python backend pipeline for model export with a Next.js frontend for interactive webcam-based detection, demonstrating how modern machine learning models can run directly in users' browsers without server-side processing.

The system features three model variants (Nano/2.6M, Small/9.4M, Medium/20.1M parameters) optimized for different speed-accuracy tradeoffs, with hardware-accelerated inference automatically selecting between WebGPU, WASM with SIMD, or fallback CPU execution. Built with Next.js 16, ONNX Runtime Web, and OpenCV.js, the application includes comprehensive letterbox preprocessing to prevent object distortion, supports 80 COCO dataset classes, and includes extensive testing with 21+ pytest tests validating model export, ONNX compliance, and inference correctness.
