# study

deepseek 671b 参数配置
https://huggingface.co/deepseek-ai/DeepSeek-R1/blob/main/config.json


LLM推理分为两个阶段：prefill阶段和 decode阶段

prefill阶段：是模型对全部的Prompt tokens一次性并行计算，最终会生成第一个输出token
decode阶段：每次生成一个token，直到生成EOS（end-of-sequence）token，产出最终的response


模型结构


Embedding层和 61层 MLA和MOE 还有一个输出层



1. Embedding层
参数量 vocab_size * hidden_size = 129280 * 7168

