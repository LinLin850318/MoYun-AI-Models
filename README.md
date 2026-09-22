# MoYun-AI-Models

墨云天气本地 AI 模型仓库（ONNX 格式，50MB 分卷存储）。

## 模型列表

| 模型 | 目录 | 大小 | 分卷数 |
|------|------|------|--------|
| Qwen1.5-0.5B-Chat (INT8) | qwen1.5-0.5b/ | 460MB | 10 |
| GPT-2 (INT8) | gpt2/ | 269MB | 6 |

## 来源

- Qwen1.5-0.5B-Chat: https://huggingface.co/Xenova/Qwen1.5-0.5B-Chat (ONNX INT8)
- GPT-2: https://huggingface.co/Xenova/gpt2 (ONNX INT8)

## 应用端使用

应用下载所有 .partNN 分卷后自动合并为 model.onnx，配合 tokenizer.json 使用 ONNX Runtime 推理。
