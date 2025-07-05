# Small Models

Comparison of small open source LLMs (8b parameters or less)

[Chat Room](#Chat-Room) | [Logic](#Logic) | [Tool Usage](#Tool-Usage) | [Vision](#Vision) | [Vision OCR](#Vision-OCR) | [Code Generation](#Code-Generation) | [General](#General)

Key:
- ✅ Pass
- ☑️ Partial Pass
- ❌ Fail
- 🕒 Fail from timeout (5 minutes)

## Chat Room

Tested with [attogram/llm-council][llm-council]

| Small Model                       | [Topic][topic]     | [Quit][quit]     |
|:----------------------------------|--------------------|------------------|
| bakllava:7b                       |                    | ❌                |
| codellama:7b                      |                    | ✅                |
| deepcoder:1.5b                    |                    | ❌                |
| deepseek-r1:1.5b                  | ❌                  | ✅                |
| deepseek-r1:8b                    |                    | ✅                |
| dolphin-mistral:7b                |                    | ✅                |
| dolphin3:8b                       |                    | ✅                |
| gemma3:1b                         |                    | ✅                |
| gemma3:4b                         | ✅                  | ✅                |
| gemma:2b                          |                    | ✅                |
| granite3.2-vision:2b              |                    | ❌                |
| granite3.3:2b                     | ❌                  | ✅                |
| huihui_ai/baronllm-abliterated:8b |                    | ✅                |
| llama3-groq-tool-use:8b           |                    | ✅                |
| llama3.2:1b                       |                    | ❌                |
| llava-llama3:8b                   |                    | ✅                |
| llava-phi3:3.8b                   |                    | ✅                |
| llava:7b                          |                    | ✅                |
| minicpm-v:8b                      |                    | ✅                |
| mistral:7b                        |                    | ✅                |
| qwen2.5-coder:7b                  |                    | ✅                |
| qwen2.5vl:3b                      |                    | ✅                |
| qwen2.5vl:7b                      |                    | ✅                |
| qwen3:1.7b                        |                    | ✅                |
| qwen3:8b                          |                    | ✅                |
| smollm2:135m                      |                    | ❌                |
| smollm2:360m                      |                    | ❌                |
| smollm2:1.7b                      |                    | ❌                |
| stable-code:3b                    |                    | ❌                |
| starcoder:7b                      |                    | ❌                |
| **Small Model**                   | **[Topic][topic]** | **[Quit][quit]** |

[quit]: <https://github.com/attogram/llm-council/blob/main/test-prompts/test.quit.txt> "Quit Test"
[topic]: <https://github.com/attogram/llm-council/blob/main/test-prompts/test.topic.txt> "Topic Test"

[^top](#Small-Models)

## Logic

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model                       | [Socrates][socrates]     | [Strawberry][strawberry]     |
|:----------------------------------|--------------------------|------------------------------|
| bakllava:7b                       | ✅                        | ❌                            |
| codellama:7b                      | ❌                        | ❌                            |
| deepcoder:1.5b                    | ✅                        | ✅                            |
| deepseek-r1:1.5b                  | ✅                        | ✅                            |
| deepseek-r1:8b                    | ✅                        | 🕒                           |
| dolphin-mistral:7b                | ✅                        | ❌                            |
| dolphin3:8b                       | ✅                        | ❌                            |
| gemma3:1b                         | ✅                        | ✅                            |
| gemma3:4b                         | ✅                        | ✅                            |
| gemma:2b                          | ✅                        | ✅                            |
| granite3.2-vision:2b              | ✅                        | ✅                            |
| granite3.3:2b                     | ✅                        | ✅                            |
| huihui_ai/baronllm-abliterated:8b | ✅                        | ❌                            |
| llama3-groq-tool-use:8b           | ✅                        | ✅                            |
| llama3.2:1b                       | ❌                        | ❌                            |
| llava-llama3:8b                   | ✅                        | ❌                            |
| llava-phi3:3.8b                   | ✅                        | ❌                            |
| llava:7b                          | ✅                        | ❌                            |
| minicpm-v:8b                      | ✅                        | ❌                            |
| mistral:7b                        | ✅                        | ❌                            |
| qwen2.5-coder:7b                  | ✅                        | ❌                            |
| qwen2.5vl:3b                      | ✅                        | ✅                            |
| qwen2.5vl:7b                      | ✅                        | ❌                            |
| qwen3:1.7b                        | ✅                        | ✅                            |
| qwen3:8b                          | ✅                        | ✅                            |
| smollm2:135m                      | ☑️                       | ❌                            |
| smollm2:360m                      | ✅                        | ❌                            |
| smollm2:1.7b                      | ✅                        | ❌                            |
| stable-code:3b                    | ❌                        | ❌                            |
| starcoder:7b                      | ❌                        | ❌                            |
| **Small Model**                   | **[Socrates][socrates]** | **[Strawberry][strawberry]** |

[socrates]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/socrates.txt> "Socrates Test"
[strawberry]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/strawberry.txt> "Strawberry Test"

[^top](#Small-Models)

## Tool Usage

Tested with [attogram/ollama-bash-toolshed][ollama-bash-toolshed]

```
granite3.3:2b
huihui_ai/baronllm-abliterated:8b
llama3.2:1b
llama3-groq-tool-use:8b
qwen3:0.6b
qwen3:1.7b
qwen3:8b *
```

[^top](#Small-Models)

## Vision

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model          | [Describe][describe] | [Keywords][keywords] | [Faces][faces] |
|:---------------------|:---------------------|----------------------|----------------|
| bakllava:7b          | ✅                    | ❌                    | ❌              |
| granite3.2-vision:2b | ✅                    | ✅                    | ❌              |
| minicpm-v:8b         | ✅                    | ✅                    | ☑️             |
| qwen2.5vl:3b         | ✅                    | ✅                    | ❌              |
| qwen2.5vl:7b         | ✅                    | ✅                    | ✅              |
| gemma3:4b            | ✅                    | ✅                    | ✅              |
| llava:7b             | ✅                    | ✅                    | ✅              |
| llava-llama3:8b      | ✅                    | ☑️                   | ☑️             |
| llava-phi3:3.8b      | ✅                    | ☑️                   | ☑️             |
| moondream:1.8b       | ✅                    | ❌                    | ❌              |

[describe]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.describe.txt> "Vision Describe Test"
[keywords]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.keywords.txt> "Vision Keywords Test"
[faces]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.faces.txt> "Vision Faces Test"

[^top](#Small-Models)

## Vision OCR

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model          | [OCR][ocr] |
|:---------------------|------------|
| bakllava:7b          | ❌          |
| granite3.2-vision:2b | ☑️         |
| minicpm-v:8b         | ☑️         |
| qwen2.5vl:3b         | ✅          |
| qwen2.5vl:7b         | ✅          |
| gemma3:4b            | 🕒         |
| llava:7b             | ❌          |
| llava-llama3:8b      | ❌          |
| llava-phi3:3.8b      | ❌          |
| moondream:1.8b       | ❌          |

[ocr]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.ocr.txt> "Vision OCR Test"

[^top](#Small-Models)

## Code Generation

| Small Model                       | [bash-1][bash-1]     | [javascript-1][javascript-1]     | [php-1][php-1]     | [python-1][python-1]     |
|:----------------------------------|----------------------|----------------------------------|--------------------|--------------------------|
| bakllava:7b                       | ❌                    |                                  |                    |                          |
| codellama:7b                      | ✅ ️                  |                                  |                    |                          |
| deepcoder:1.5b                    | ❌                    |                                  |                    |                          |
| deepseek-r1:1.5b                  | ❌                    |                                  |                    |                          |
| deepseek-r1:8b                    | 🕒                   |                                  |                    |                          |
| dolphin-mistral:7b                | ✅                    |                                  |                    |                          |
| dolphin3:8b                       | ✅                    |                                  |                    |                          |
| gemma3:1b                         | ☑️                   |                                  |                    |                          |
| gemma3:4b                         | ☑️                   |                                  |                    |                          |
| gemma:2b                          | ✅                    |                                  |                    |                          |
| granite3.2-vision:2b              | ✅                    |                                  |                    |                          |
| granite3.3:2b                     | ☑️                   |                                  |                    |                          |
| huihui_ai/baronllm-abliterated:8b | ✅                    |                                  |                    |                          |
| llama3-groq-tool-use:8b           | ✅                    |                                  |                    |                          |
| llama3.2:1b                       | ☑️                   |                                  |                    |                          |
| llava-llama3:8b                   | ☑️                   |                                  |                    |                          |
| llava-phi3:3.8b                   | ✅                    |                                  |                    |                          |
| llava:7b                          | ✅                    |                                  |                    |                          |
| minicpm-v:8b                      | ❌                    |                                  |                    |                          |
| mistral:7b                        | ☑️                   |                                  |                    |                          |
| qwen2.5-coder:7b                  | ✅                    |                                  |                    |                          |
| qwen2.5vl:3b                      | ☑️                   |                                  |                    |                          |
| qwen2.5vl:7b                      | ✅                    |                                  |                    |                          |
| qwen3:1.7b                        | ✅                    |                                  |                    |                          |
| qwen3:8b                          | ✅                    |                                  |                    |                          |
| smollm2:135m                      | ❌                    |                                  |
| smollm2:360m                      | ☑️                   |                                  |
| smollm2:1.7b                      | ✅                    |                                  |
| stable-code:3b                    | ☑️                   |                                  |                    |                          |
| starcoder:7b                      | ☑️                   |                                  |                    |                          |
| **Small Model**                   | **[bash-1][bash-1]** | **[javascript-1][javascript-1]** | **[php-1][php-1]** | **[python-1][python-1]** |

[bash-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/bash.array.to.html.txt> "Bash Array to HTML Test"
[javascript-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/javascript.array.to.html.txt> "Javascript Array to HTML Test"
[php-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/php.array.to.html.txt> "PHP Array to HTML Test"
[python-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/python.array.to.html.txt> "Python Array to HTML Test"

[^top](#Small-Models)

## General

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model                       | [Hovercraft][hovercraft]     | [Who][who]     |
|:----------------------------------|------------------------------|----------------|
| bakllava:7b                       | ❌                            | ✅              |
| codellama:7b                      | ✅                            | ✅              |
| deepcoder:1.5b                    | ✅                            | ✅              |
| deepseek-r1:1.5b                  | ✅                            | ✅              |
| deepseek-r1:8b                    | ☑️   ️                       | ✅              |
| dolphin-mistral:7b                | ☑️                           | ✅              |
| dolphin3:8b                       | ✅                            | ✅              |
| gemma3:1b                         | ☑️                           | ✅              |
| gemma3:4b                         | ☑️                           | ✅              |
| gemma:2b                          | ☑️                           | ✅              |
| granite3.2-vision:2b              | ✅                            | ✅              |
| granite3.3:2b                     | ☑️                           | ✅              |
| huihui_ai/baronllm-abliterated:8b | ☑️                           | ✅              |
| llama3-groq-tool-use:8b           | ☑️                           | ✅              |
| llama3.2:1b                       | ✅                            | ☑️             |
| llava-llama3:8b                   | ☑️                           | ✅              |
| llava-phi3:3.8b                   | ✅                            | ✅              |
| llava:7b                          | ✅                            | ✅              |
| minicpm-v:8b                      | ❌                            | ✅              |
| mistral:7b                        | ☑️                           | ✅              |
| qwen2.5-coder:7b                  | ✅                            | ✅              |
| qwen2.5vl:3b                      | ✅                            | ✅              |
| qwen2.5vl:7b                      | ☑️                           | ✅              |
| qwen3:1.7b                        | ✅                            | ✅              |
| qwen3:8b                          | ☑️                           | ✅              |
| smollm2:135m                      | ✅                            | ✅              |
| smollm2:360m                      | ☑️                           | ✅              |
| smollm2:1.7b                      | ✅                            | ✅              |
| stable-code:3b                    | ☑️                           | ✅              |
| starcoder:7b                      | ❌                            | ❌              |
| **Small Model**                   | **[Hovercraft][hovercraft]** | **[Who][who]** |

[hovercraft]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/hovercraft.txt> "Hovercraft Test"
[who]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/who.are.you.txt> "Who are you Test"

```
deepseek-r1:7b
llama3.1:8b
llama3.3:3b
llama3:8b
phi:2.7b
phi3:3.8b
tinyllama:1.1b
qwen3:0.6b
qwen3:4b
```

[^top](#Small-Models)

## Attogram Artificial Intelligence Projects

* [ollama-multirun](https://github.com/attogram/ollama-multirun) — A bash shell script to run a single prompt against any or all of your locally installed ollama models, saving the output and performance statistics as easily navigable web pages.
* [llm-council](https://github.com/attogram/llm-council) — A bash script to start a chat between 2 or more LLMs running on ollama
* [ollama-bash-toolshed](https://github.com/attogram/ollama-bash-toolshed) — A bash script to chat with tool usage models.  Easily add new tools to your shed!
* [small-models](https://github.com/attogram/small-models) — Comparison of small open source LLMs
* [AI Test Zone](https://github.com/attogram/ai_test_zone) — Demos hosted on https://attogram.github.io/ai_test_zone/

[llm-council]: <https://github.com/attogram/llm-council> "LLM Council"
[ollama-bash-toolshed]: <https://github.com/attogram/ollama-bash-toolshed> "Ollama Bash Toolshed"
[ollama-multirun]: <https://github.com/attogram/ollama-multirun> "Ollama Multirun"
