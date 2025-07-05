<a id="top"></a>
# Small Models

Comparison of small open source LLMs (8b parameters or less)

[Chat Room](#Chat-Room) | [Logic](#Logic) | [Tool Usage](#Tool-Usage) | [Vision](#Vision) | [Vision OCR](#Vision-OCR) | [Code Generation](#Code-Generation) | [General](#General)

## Chat Room

Tested with [attogram/llm-council](https://github.com/attogram/llm-council)

| Small Model                                      | [Quit][101] |
|:-------------------------------------------------|:-----------:|
| bakllava:7b                                      |      ❌      |
| codellama:7b                                     |      ✅      |
| deepcoder:1.5b                                   |      ❌      |
| deepseek-r1:1.5b                                 |      ✅      |
| deepseek-r1:8b                                   |      ✅      |
| dolphin-mistral:7b                               |      ✅      |
| dolphin3:8b                                      |      ✅      |
| gemma3:1b                                        |      ✅      |
| gemma3:4b                                        |      ✅      |
| gemma:2b                                         |      ✅      |
| granite3.2-vision:2b                             |      ❌      |
| granite3.3:2b                                    |      ✅      |
| <small>huihui_ai/baronllm-abliterated:8b</small> |      ✅      |
| llama3-groq-tool-use:8b                          |      ✅      |
| llama3.2:1b                                      |      ❌      |
| llava-llama3:8b                                  |      ✅      |
| llava-phi3:3.8b                                  |      ✅      |
| llava:7b                                         |      ✅      |
| minicpm-v:8b                                     |      ✅      |
| mistral:7b                                       |      ✅      |
| qwen2.5-coder:7b                                 |      ✅      |
| qwen2.5vl:3b                                     |      ✅      |
| qwen2.5vl:7b                                     |      ✅      |
| qwen3:1.7b                                       |      ✅      |
| qwen3:8b                                         |      ✅      |
| smollm2:135m                                     |      ❌      |
| smollm2:360m                                     |      ❌      |
| smollm2:1.7b                                     |      ❌      |
| stable-code:3b                                   |      ❌      |
| starcoder:7b                                     |      ❌      |

[101]: <https://github.com/attogram/llm-council/blob/main/test-prompts/test.quit.txt> "Quit Test"

[^top](#top)

## Logic

Tested with [attogram/ollama-multirun](https://github.com/attogram/ollama-multirun)

| Small Model                                      | [Socrates][201] | [Strawberry][202] |
|:-------------------------------------------------|:---------------:|:-----------------:|
| bakllava:7b                                      |        ✅        |         ❌         |
| codellama:7b                                     |        ❌        |         ❌         |
| deepcoder:1.5b                                   |        ✅        |         ✅         |
| deepseek-r1:1.5b                                 |        ✅        |         ✅         |
| deepseek-r1:8b                                   |        ✅        |        🕒         |
| dolphin-mistral:7b                               |        ✅        |         ❌         |
| dolphin3:8b                                      |        ✅        |         ❌         |
| gemma3:1b                                        |        ✅        |         ✅         |
| gemma3:4b                                        |        ✅        |         ✅         |
| gemma:2b                                         |        ✅        |         ✅         |
| granite3.2-vision:2b                             |        ✅        |         ✅         |
| granite3.3:2b                                    |        ✅        |         ✅         |
| <small>huihui_ai/baronllm-abliterated:8b</small> |        ✅        |         ❌         |
| llama3-groq-tool-use:8b                          |        ✅        |         ✅         |
| llama3.2:1b                                      |        ❌        |         ❌         |
| llava-llama3:8b                                  |        ✅        |         ❌         |
| llava-phi3:3.8b                                  |        ✅        |         ❌         |
| llava:7b                                         |        ✅        |         ❌         |
| minicpm-v:8b                                     |        ✅        |         ❌         |
| mistral:7b                                       |        ✅        |         ❌         |
| qwen2.5-coder:7b                                 |        ✅        |         ❌         |
| qwen2.5vl:3b                                     |        ✅        |         ✅         |
| qwen2.5vl:7b                                     |        ✅        |         ❌         |
| qwen3:1.7b                                       |        ✅        |         ✅         |
| qwen3:8b                                         |        ✅        |         ✅         |
| smollm2:135m                                     |        -        |         -         |
| smollm2:360m                                     |        -        |         -         |
| smollm2:1.7b                                     |        -        |         -         |
| stable-code:3b                                   |        ❌        |         ❌         |
| starcoder:7b                                     |        ❌        |         ❌         |

[201]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/socrates.txt> "Socrates Test"
[202]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/strawberry.txt> "Strawberry Test"

[^top](#top)

## Tool Usage

Tested with [attogram/ollama-bash-toolshed](https://github.com/attogram/ollama-bash-toolshed)

```
granite3.3:2b
huihui_ai/baronllm-abliterated:8b
llama3.2:1b
llama3-groq-tool-use:8b
qwen3:0.6b
qwen3:1.7b
qwen3:8b *
```

[^top](#top)

## Vision
```
bakllava:7b
gemma3:1b
gemma3:4b
granite3.2-vision:2b 
llava-llama3:8b
llava-phi3:3.8b 
llava:7b 
minicpm-v:8b *
moondream:1.8b
qwen2.5vl:3b 
qwen2.5vl:7b
```

[^top](#top)

## Vision OCR
```
granite3.2-vision:2b
minicpm-v:8b
qwen2.5vl:7b
```

[^top](#top)

## Code Generation
```
codellama:7b
deepcoder:1.5b
dolphin3:8b
gemma:2b
granite3.3:2b
mistral:7b
qwen2.5-coder:7b
qwen3:1.7b
stable-code:3b
starcoder:7b
```

[^top](#top)

## General
```
deepseek-r1:1.5b
deepseek-r1:7b
deepseek-r1:8b
dolphin3:8b
gemma:2b
gemma3:1b
gemma3:4b
granite3.3:2b
llama3.1:8b
llama3.2:1b
llama3.3:3b
llama3:8b
llava-llama3:8b
llava-phi3:3.8b
llava:7b
mistral:7b
phi:2.7b
phi3:3.8b
tinyllama:1.1b
qwen3:0.6b
qwen3:1.7b
qwen3:4b
qwen3:8b
smollm2:135m
smollm2:360m
smollm2:1.7b
```

[^top](#top)

## Attogram Artificial Intelligence Projects

* [ollama-multirun](https://github.com/attogram/ollama-multirun) — A bash shell script to run a single prompt against any or all of your locally installed ollama models, saving the output and performance statistics as easily navigable web pages.
* [llm-council](https://github.com/attogram/llm-council) — A bash script to start a chat between 2 or more LLMs running on ollama
* [ollama-bash-toolshed](https://github.com/attogram/ollama-bash-toolshed) — A bash script to chat with tool usage models.  Easily add new tools to your shed!
* [small-models](https://github.com/attogram/small-models) — Comparison of small open source LLMs
* [AI Test Zone](https://github.com/attogram/ai_test_zone) — Demos hosted on https://attogram.github.io/ai_test_zone/
