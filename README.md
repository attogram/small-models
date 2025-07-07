# Small Models

Comparison of small open source LLMs (8b parameters or less)

[Tool Usage](#Tool-Usage) | [Chat Room](#Chat-Room) | [Logic](#Logic) | [Vision](#Vision) | [Vision OCR](#Vision-OCR) | [Code Generation](#Code-Generation) | [General](#General)

All testing done with [Ollama](https://github.com/ollama/ollama)

Key:
- ✅ Pass
- ☑️ Partial Pass
- ❌ Fail
- 🕒 Fail from timeout (5 minutes)

## Tool Usage

Tested with [attogram/ollama-bash-toolshed][ollama-bash-toolshed]

| Passing       | [Math][math] | [Ollama][ollama] | [Time][time] | [Web][web] |
|:--------------|:------------:|:----------------:|:------------:|:----------:|
| cogito:8b     |      ✅       |        ✅         |      ✅       |     ✅      |
| granite3.3:2b |      ✅       |        ✅         |      ✅       |     ✅      |
| hermes3:8b    |      ✅       |        ✅         |      ✅       |     ✅      |
| llama3.2:1b   |      ✅       |        ✅         |      ✅       |     ✅      |
| llama3.2:3b   |      ✅       |        ✅         |      ✅       |     ✅      |
| qwen3:1.7b    |      ✅       |        ✅         |      ✅       |     ✅      |
| qwen3:4b      |      ✅       |        ✅         |      ✅       |     ✅      |
| qwen3:8b      |      ✅       |        ✅         |      ✅       |     ✅      |

| Failing                 | [Math][math] | [Ollama][ollama] | [Time][time] | [Web][web] |
|:------------------------|:------------:|:----------------:|:------------:|:----------:|
| command-r7b:7b          |      ❌       |        ❌         |      ❌       |     ❌      |
| granite3.2-vision:2b    |      ❌       |        ❌         |      ❌       |     ❌      |
| llama3-groq-tool-use:8b |      ✅       |        ✅         |      ❌       |     ✅      |
| mistral:7b              |      ❌       |        ❌         |      ❌       |     ❌      |
| nemotron-mini:4b        |      ✅       |        ❌         |      ✅       |     ☑️     |
| qwen2.5-coder:7b        |      ☑️      |        ☑️        |      ☑️      |     ☑️     |
| qwen3:0.6b              |      ✅       |        ☑️        |      ❌       |     ✅      |
| smollm2:1.7b            |      ☑️      |        ❌         |      ☑️      |     ☑️     |

[math]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/math.txt> "Webpage Tool Test"
[ollama]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/ollama.txt> "Ollama Tool Test"
[time]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/time.txt> "Datetime Tool Test"
[web]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/web.txt> "What time is it Test"

```
aya-expanse:8b
cogito:3b
command-r7b-arabic:7b
granite3-dense:2b
granite3-dense:8b
granite3-moe:1b
granite3-moe:3b
granite3.1-dense:2b
granite3.1-dense:8b
granite3.1-moe:1b
granite3.1-moe:3b
granite3.2:2b
granite3.2:8b
granite3.3:8b
hermes3:3b
llama3.1:8b
mixtral:8x7b
phi4-mini:3.8b
qwen2.5-coder:0.5b
qwen2.5-coder:1.5b
qwen2.5-coder:3b
qwen2.5:0.5b
qwen2.5:1.5b
qwen2.5:3b
qwen2.5:7b
qwen2:0.5b
qwen2:1.5b
qwen2:7b

Hituzip/gemma3-tools:4b
PetrosStav/gemma3-tools:4b
hhao/qwen2.5-coder-tools:0.5b
hhao/qwen2.5-coder-tools:1.5b
hhao/qwen2.5-coder-tools:3b
hhao/qwen2.5-coder-tools:7b
ishumilin/deepseek-r1-coder-tools-tuned:1.5b
ishumilin/deepseek-r1-coder-tools-tuned:7b
ishumilin/deepseek-r1-coder-tools-tuned:8b
ishumilin/deepseek-r1-coder-tools:1.5b
ishumilin/deepseek-r1-coder-tools:7b
ishumilin/deepseek-r1-coder-tools:8b
maryasov/qwen2.5-coder-cline:7b
orieg/gemma3-tools:1b
orieg/gemma3-tools:4b
tom_himanen/deepseek-r1-roo-cline-tools:1.5b
tom_himanen/deepseek-r1-roo-cline-tools:7b
tom_himanen/deepseek-r1-roo-cline-tools:8b
```
[^top](#Small-Models)

## Chat Room

Tested with [attogram/llm-council][llm-council]

| Small Model                       | [Peace][peace]     | [Quit][quit]     | [Topic][topic]     |
|:----------------------------------|--------------------|------------------|--------------------|
| bakllava:7b                       |                    | ❌                |                    |
| codellama:7b                      |                    | ✅                |                    |
| deepcoder:1.5b                    |                    | ❌                |                    |
| deepseek-r1:1.5b                  |                    | ✅                | ❌                  |
| deepseek-r1:8b                    |                    | ✅                |                    |
| dolphin-mistral:7b                |                    | ✅                |                    |
| dolphin3:8b                       | ✅                  | ✅                |                    |
| gemma3:1b                         |                    | ✅                |                    |
| gemma3:4b                         | ✅                  | ✅                | ✅                  |
| gemma:2b                          |                    | ✅                |                    |
| granite3.2-vision:2b              |                    | ❌                |                    |
| granite3.3:2b                     | ✅                  | ✅                | ❌                  |
| huihui_ai/baronllm-abliterated:8b |                    | ✅                |                    |
| llama3-groq-tool-use:8b           |                    | ✅                |                    |
| llama3.2:1b                       |                    | ❌                |                    |
| llava-llama3:8b                   |                    | ✅                |                    |
| llava-phi3:3.8b                   |                    | ✅                |                    |
| llava:7b                          |                    | ✅                |                    |
| minicpm-v:8b                      | ✅                  | ✅                |                    |
| mistral:7b                        | ✅                  | ✅                |                    |
| qwen2.5-coder:7b                  |                    | ✅                |                    |
| qwen2.5vl:3b                      |                    | ✅                |                    |
| qwen2.5vl:7b                      |                    | ✅                |                    |
| qwen3:1.7b                        |                    | ✅                |                    |
| qwen3:8b                          | ✅                  | ✅                |                    |
| smollm2:135m                      |                    | ❌                |                    |
| smollm2:360m                      |                    | ❌                |                    |
| smollm2:1.7b                      |                    | ❌                |                    |
| stable-code:3b                    |                    | ❌                |                    |
| starcoder:7b                      |                    | ❌                |                    |
| **Small Model**                   | **[Peace][peace]** | **[Quit][quit]** | **[Topic][topic]** |

[quit]: <https://github.com/attogram/llm-council/blob/main/test-prompts/test.quit.txt> "Quit Test"
[peace]: <https://github.com/attogram/llm-council/blob/main/test-prompts/world.peace.txt> "World Peace Test"
[topic]: <https://github.com/attogram/llm-council/blob/main/test-prompts/test.topic.txt> "Topic Test"

[^top](#Small-Models)

## Logic

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model                       |   [Socrates][socrates]   |   [Strawberry][strawberry]   |
|:----------------------------------|:------------------------:|:----------------------------:|
| bakllava:7b                       |            ✅             |              ❌               |
| ~~codellama:7b~~                  |            ❌             |              ❌               |
| **deepcoder:1.5b**                |            ✅             |              ✅               |
| **deepseek-r1:1.5b**              |            ✅             |              ✅               |
| deepseek-r1:8b                    |            ✅             |              🕒              |
| dolphin-mistral:7b                |            ✅             |              ❌               |
| dolphin3:8b                       |            ✅             |              ❌               |
| **gemma3:1b**                     |            ✅             |              ✅               |
| **gemma3:4b**                     |            ✅             |              ✅               |
| **gemma:2b**                      |            ✅             |              ✅               |
| **granite3.2-vision:2b**          |            ✅             |              ✅               |
| **granite3.3:2b**                 |            ✅             |              ✅               |
| huihui_ai/baronllm-abliterated:8b |            ✅             |              ❌               |
| **llama3-groq-tool-use:8b**       |            ✅             |              ✅               |
| ~~llama3.2:1b~~                   |            ❌             |              ❌               |
| llava-llama3:8b                   |            ✅             |              ❌               |
| llava-phi3:3.8b                   |            ✅             |              ❌               |
| llava:7b                          |            ✅             |              ❌               |
| minicpm-v:8b                      |            ✅             |              ❌               |
| mistral:7b                        |            ✅             |              ❌               |
| qwen2.5-coder:7b                  |            ✅             |              ❌               |
| **qwen2.5vl:3b**                  |            ✅             |              ✅               |
| qwen2.5vl:7b                      |            ✅             |              ❌               |
| **qwen3:1.7b**                    |            ✅             |              ✅               |
| **qwen3:8b**                      |            ✅             |              ✅               |
| smollm2:135m                      |            ☑️            |              ❌               |
| smollm2:360m                      |            ✅             |              ❌               |
| smollm2:1.7b                      |            ✅             |              ❌               |
| ~~stable-code:3b~~                |            ❌             |              ❌               |
| ~~starcoder:7b~~                  |            ❌             |              ❌               |
| **Small Model**                   | **[Socrates][socrates]** | **[Strawberry][strawberry]** |

[socrates]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/socrates.txt> "Socrates Test"
[strawberry]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/strawberry.txt> "Strawberry Test"

[^top](#Small-Models)

## Vision

Tested with [attogram/ollama-multirun][ollama-multirun]

| Passing              | [Describe][describe] | [Keywords][keywords] | [Faces][faces] |
|:---------------------|:--------------------:|:--------------------:|:--------------:|
| bakllava:7b          |          ✅           |          ❌           |       ❌        |
| granite3.2-vision:2b |          ✅           |          ✅           |       ❌        |
| minicpm-v:8b         |          ✅           |          ✅           |       ☑️       |
| qwen2.5vl:3b         |          ✅           |          ✅           |       ❌        |
| **qwen2.5vl:7b**     |          ✅           |          ✅           |       ✅        |
| **gemma3:4b**        |          ✅           |          ✅           |       ✅        |
| **llava:7b**         |          ✅           |          ✅           |       ✅        |
| llava-llama3:8b      |          ✅           |          ☑️          |       ☑️       |
| llava-phi3:3.8b      |          ✅           |          ☑️          |       ☑️       |
| moondream:1.8b       |          ✅           |          ❌           |       ❌        |

[describe]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.describe.txt> "Vision Describe Test"
[keywords]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.keywords.txt> "Vision Keywords Test"
[faces]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.faces.txt> "Vision Faces Test"

[^top](#Small-Models)

## Vision OCR

Tested with [attogram/ollama-multirun][ollama-multirun]

| Passing              | [OCR][ocr] |
|:---------------------|:----------:|
| granite3.2-vision:2b |     ☑️     |
| minicpm-v:8b         |     ☑️     |
| **qwen2.5vl:3b**     |     ✅      |
| **qwen2.5vl:7b**     |     ✅      |

| Failing              | [OCR][ocr] |
|:---------------------|:----------:|
| ~~bakllava:7b~~      |     ❌      |
| gemma3:4b            |     🕒     |
| ~~llava:7b~~         |     ❌      |
| ~~llava-llama3:8b~~  |     ❌      |
| ~~llava-phi3:3.8b~~  |     ❌      |
| ~~moondream:1.8b~~   |     ❌      |

[ocr]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision.ocr.txt> "Vision OCR Test"

[^top](#Small-Models)

## Code Generation

| Small Model                           |   [bash-1][bash-1]   |   [js-1][js-1]   |   [php-1][php-1]   |   [python-1][python-1]   |
|:--------------------------------------|:--------------------:|:----------------:|:------------------:|:------------------------:|
| bakllava:7b                           |          ❌           |                  |         ☑️         |                          |
| **codellama:7b**                      |         ✅ ️          |                  |         ✅          |                          |
| deepcoder:1.5b                        |          ❌           |                  |         ✅          |                          |
| deepseek-r1:1.5b                      |          ❌           |                  |         ✅          |                          |
| deepseek-r1:8b                        |          🕒          |                  |         🕒         |                          |
| **dolphin-mistral:7b**                |          ✅           |                  |         ✅          |                          |
| **dolphin3:8b**                       |          ✅           |                  |         ✅          |                          |
| gemma3:1b                             |          ☑️          |                  |         ☑️         |                          |
| gemma3:4b                             |          ☑️          |                  |         ✅          |                          |
| gemma:2b                              |          ✅           |                  |         ❌          |                          |
| **granite3.2-vision:2b**              |          ✅           |                  |         ✅          |                          |
| granite3.3:2b                         |          ☑️          |                  |         ✅          |                          |
| **huihui_ai/baronllm-abliterated:8b** |          ✅           |                  |         ✅          |                          |
| **llama3-groq-tool-use:8b**           |          ✅           |                  |         ✅          |                          |
| llama3.2:1b                           |          ☑️          |                  |         ☑️         |                          |
| llava-llama3:8b                       |          ☑️          |                  |         ✅          |                          |
| **llava-phi3:3.8b**                   |          ✅           |                  |         ✅          |                          |
| **llava:7b**                          |          ✅           |                  |         ✅          |                          |
| minicpm-v:8b                          |          ❌           |                  |         ✅          |                          |
| mistral:7b                            |          ☑️          |                  |         ✅          |                          |
| **qwen2.5-coder:7b**                  |          ✅           |                  |         ✅          |                          |
| qwen2.5vl:3b                          |          ☑️          |                  |         ✅          |                          |
| **qwen2.5vl:7b**                      |          ✅           |                  |         ✅          |                          |
| **qwen3:1.7b**                        |          ✅           |                  |         ✅          |                          |
| **qwen3:8b**                          |          ✅           |                  |         ✅          |                          |
| ~~smollm2:135m~~                      |          ❌           |                  |         ❌          |                          |
| smollm2:360m                          |          ☑️          |                  |         ☑️         |                          |
| smollm2:1.7b                          |          ✅           |                  |         ☑️         |                          |
| stable-code:3b                        |          ☑️          |                  |         ✅          |                          |
| starcoder:7b                          |          ☑️          |                  |         ❌          |                          |
| **Small Model**                       | **[bash-1][bash-1]** | **[js-1][js-1]** | **[php-1][php-1]** | **[python-1][python-1]** |

[bash-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/bash.array.to.html.txt> "Bash Array to HTML Test"
[js-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/javascript.array.to.html.txt> "Javascript Array to HTML Test"
[php-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/php.array.to.html.txt> "PHP Array to HTML Test"
[python-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/python.array.to.html.txt> "Python Array to HTML Test"

[^top](#Small-Models)

## General

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model                       |   [Hovercraft][hovercraft]   |   [Who][who]   |
|:----------------------------------|:----------------------------:|:--------------:|
| bakllava:7b                       |              ❌               |       ✅        |
| **codellama:7b**                  |              ✅               |       ✅        |
| **deepcoder:1.5b**                |              ✅               |       ✅        |
| **deepseek-r1:1.5b**              |              ✅               |       ✅        |
| deepseek-r1:8b                    |              ☑️              |       ✅        |
| dolphin-mistral:7b                |              ☑️              |       ✅        |
| **dolphin3:8b**                   |              ✅               |       ✅        |
| gemma3:1b                         |              ☑️              |       ✅        |
| gemma3:4b                         |              ☑️              |       ✅        |
| gemma:2b                          |              ☑️              |       ✅        |
| **granite3.2-vision:2b**          |              ✅               |       ✅        |
| granite3.3:2b                     |              ☑️              |       ✅        |
| huihui_ai/baronllm-abliterated:8b |              ☑️              |       ✅        |
| llama3-groq-tool-use:8b           |              ☑️              |       ✅        |
| **llama3.2:1b**                   |              ✅               |       ☑️       |
| llava-llama3:8b                   |              ☑️              |       ✅        |
| **llava-phi3:3.8b**               |              ✅               |       ✅        |
| **llava:7b**                      |              ✅               |       ✅        |
| minicpm-v:8b                      |              ❌               |       ✅        |
| mistral:7b                        |              ☑️              |       ✅        |
| **qwen2.5-coder:7b**              |              ✅               |       ✅        |
| **qwen2.5vl:3b**                  |              ✅               |       ✅        |
| qwen2.5vl:7b                      |              ☑️              |       ✅        |
| **qwen3:1.7b**                    |              ✅               |       ✅        |
| qwen3:8b                          |              ☑️              |       ✅        |
| **smollm2:135m**                  |              ✅               |       ✅        |
| smollm2:360m                      |              ☑️              |       ✅        |
| **smollm2:1.7b**                  |              ✅               |       ✅        |
| stable-code:3b                    |              ☑️              |       ✅        |
| ~~starcoder:7b~~                  |              ❌               |       ❌        |
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
