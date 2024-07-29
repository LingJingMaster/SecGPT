# SecGPT
### **项目**
- [GitHub](https://github.com/Clouditera/SecGPT)
- [原版Pytorch模型](https://huggingface.co/clouditera/secgpt)
### **简介**
- 随着大语言模型的崛起，网安大模型也掀起了一股热潮，本人在逛 GitHub 时偶然发现了云起无垠开源的 SecGPT，但官方调用脚本中使用了 Cuda，且没有提供 GGUF 版本，故使用了 [llama.cpp](https://github.com/ggerganov/llama.cpp) 的 convert 脚本进行转换，并上传至huggingface

### **测试设备**
- MacBook Pro 16 寸
- M3 Max
- 48 GB

### **Usage**
- 分为 `secgpt1.5.gguf` , `secgpt.gguf` 与 `secgpt-mini.gguf` 三个版本
    - `secgpt1.5.gguf`基于qwen2,    需 28.5 G 显存
	- `secgpt.gguf`基于baichuan,   需 26.5 G 显存
	- `secgpt-mini.gguf`基于qwen2, 需 1.6 G 显存
- 使用方法
	- 将 GGUF 导入[LM Studio](https://lmstudio.ai/)，并使用 `secgpt-all.json` 作为参数配置
