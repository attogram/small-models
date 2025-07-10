# Small Models

Comparison of small open source LLMs (8b parameters or less)

[General](#General) | [Tool Usage](#Tool-Usage) | [Chat Room](#Chat-Room) | [Logic](#Logic) | [Vision](#Vision) | [Vision OCR](#Vision-OCR) | [Code Generation](#Code-Generation) | [More](#More-from-the-Attogram-Project)

All testing done with [Ollama](https://github.com/ollama/ollama) on a MacBook Pro with Apple M2 chip and 16 GB memory.

|       | Key                              |
|:-----:|:---------------------------------|
|   ✅   | Pass                             |
|  ☑️   | Partial Pass                     |
|   ❌   | Fail                             |
|  🕒   | Timeout                          |
| 😵‍💫 | Hallucinations                   |
|  🚫   | Rejected prompt / unsafe content |
|  💔   | Malformed Response / Tool call   |

## General

Tested with [attogram/ollama-multirun][ollama-multirun]

| Small Model                       |   [Hovercraft][hovercraft]   | [Pirate][pirate]                                                                                                                       |   [Who][who]   |
|:----------------------------------|:----------------------------:|----------------------------------------------------------------------------------------------------------------------------------------|:--------------:|
| bakllava:7b                       |              ❌               |                                                                                                                                        |       ✅        |
| codellama:7b                      |              ✅               | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/codellama_7b.html)       |       ✅        |
| cogito:3b                         |                              | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/cogito_3b.html)          |       ✅        |
| cogito:bb                         |                              | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/cogito_8b.html)          |       ✅        |
| deepcoder:1.5b                    |              ✅               | [☑️](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/deepcoder_1_5b.html)    |       ✅        |
| deepseek-r1:1.5b                  |              ✅               | [☑️](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/deepseek_r1_1_5b.html)  |       ✅        |
| deepseek-r1:8b                    |              ☑️              | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/deepseek_r1_8b.html)     |       ✅        |
| dolphin-mistral:7b                |              ☑️              | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/dolphin_mistral_7b.html) |       ✅        |
| dolphin3:8b                       |              ✅               | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/dolphin3_8b.html)        |       ✅        |
| gemma3:1b                         |              ☑️              | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/gemma3_1b.html)          |       ✅        |
| gemma3:4b                         |              ☑️              |                                                                                                                                        |       ✅        |
| gemma:2b                          |              ☑️              |                                                                                                                                        |       ✅        |
| granite3.2-vision:2b              |              ✅               |                                                                                                                                        |       ✅        |
| granite3.3:2b                     |              ☑️              |                                                                                                                                        |       ✅        |
| huihui_ai/baronllm-abliterated:8b |              ☑️              |                                                                                                                                        |       ✅        |
| llama3-groq-tool-use:8b           |              ☑️              |                                                                                                                                        |       ✅        |
| llama3.2:1b                       |              ✅               |                                                                                                                                        |       ☑️       |
| llava-llama3:8b                   |              ☑️              |                                                                                                                                        |       ✅        |
| llava-phi3:3.8b                   |              ✅               |                                                                                                                                        |       ✅        |
| llava:7b                          |              ✅               |                                                                                                                                        |       ✅        |
| minicpm-v:8b                      |              ❌               |                                                                                                                                        |       ✅        |
| mistral:7b                        |              ☑️              |                                                                                                                                        |       ✅        |
| qwen2.5-coder:7b                  |              ✅               |                                                                                                                                        |       ✅        |
| qwen2.5vl:3b                      |              ✅               |                                                                                                                                        |       ✅        |
| qwen2.5vl:7b                      |              ☑️              |                                                                                                                                        |       ✅        |
| qwen3:1.7b                        |              ✅               | [🕒](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/qwen3_1_7b.html)        |       ✅        |
| qwen3:4b                          |              ✅               | [🕒](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/qwen3_4b.html)          |       ✅        |
| qwen3:8b                          |              ☑️              | [✅](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/qwen3_8b.html)           |       ✅        |
| smollm2:135m                      |              ✅               |                                                                                                                                        |       ✅        |
| smollm2:360m                      |              ☑️              |                                                                                                                                        |       ✅        |
| smollm2:1.7b                      |              ✅               |                                                                                                                                        |       ✅        |
| stable-code:3b                    |              ☑️              | [☑️](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/stable_code_3b.html)    |       ✅        |
| starcoder:7b                      |              ❌               | [❌](https://attogram.github.io/ai_test_zone/from_now_on_you_must_talk_like_a_pirate_arg__tell_20250710-195750/starcoder_7b.html)       |       ❌        |
| **Small Model**                   | **[Hovercraft][hovercraft]** | **[Pirate][pirate]**                                                                                                                   | **[Who][who]** |

[hovercraft]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/general/hovercraft.txt> "Hovercraft Test"
[pirate]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/general/pirate.jokes.txt> "Pirate jokes Test"
[who]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/general/who.are.you.txt> "Who are you Test"

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

## Tool Usage

Tested with [attogram/ollama-bash-toolshed][ollama-bash-toolshed]

| Passing       | [Math][math] | [Ollama][ollama] | [Time][time] | [Web][web] |
|:--------------|:------------:|:----------------:|:------------:|:----------:|
| cogito:3b     |      ✅       |        ✅         |      ✅       |     ✅      |
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
| granite3.3:8b           |      💔      |        💔        |      💔      |     💔     |
| llama3-groq-tool-use:8b |      ✅       |        ✅         |      ❌       |     ✅      |
| mistral:7b              |      💔      |        💔        |      💔      |     💔     |
| nemotron-mini:4b        |      ✅       |        ❌         |      ✅       |     ☑️     |
| qwen2.5-coder:7b        |      💔      |        💔        |      💔      |     💔     |
| qwen3:0.6b              |      ✅       |        ☑️        |      ❌       |     ✅      |
| smollm2:1.7b            |      💔      |        💔        |      ✅       |   😵‍💫    |

[math]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/math.txt> "Math Tool Test"
[ollama]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/ollama.txt> "Ollama Tool Test"
[time]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/time.txt> "Datetime Tool Test"
[web]: <https://github.com/attogram/ollama-bash-toolshed/blob/main/test-prompts/web.txt> "Web Tool Test"

```
aya-expanse:8b
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

[socrates]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/logic/socrates.txt> "Socrates Test"
[strawberry]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/logic/strawberry.txt> "Strawberry Test"

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

[describe]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision/vision.describe.txt> "Vision Describe Test"
[keywords]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision/vision.keywords.txt> "Vision Keywords Test"
[faces]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision/vision.faces.txt> "Vision Faces Test"

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

[ocr]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/vision/vision.ocr.txt> "Vision OCR Test"

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

[bash-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/code/bash.array.to.html.txt> "Bash Array to HTML Test"
[js-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/code/javascript.array.to.html.txt> "Javascript Array to HTML Test"
[php-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/code/php.array.to.html.txt> "PHP Array to HTML Test"
[python-1]: <https://github.com/attogram/ollama-multirun/blob/main/test-prompts/code/python.array.to.html.txt> "Python Array to HTML Test"

[^top](#Small-Models)

## More from the Attogram Project

| Project               | Github Repo                                      | Description                                                                                                                                                                                 |
|-----------------------|--------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Multirun**          | [ollama-multirun][ollama-multirun]               | run a prompt against all, or some, of your models running on Ollama.<br />Creates web pages with the output, performance statistics and model info.<br />All in a single Bash shell script. |
| **Toolshed**          | [ollama-bash-toolshed][ollama-bash-toolshed]     | chat with tool calling models. Sample tools included.<br />Add new tools to your shed with ease. Runs on Ollama.<br />All via Bash shell scripts.                                           |
| **LLM Council**       | [llm-council][llm-council]                       | start a chat room between all, or some, of your models running on Ollama.<br />All in a single Bash shell script.                                                                           |
| **Small Models**      | [small-models][small-models]                     | a comparison of small open source LLMs (8b parameters or less)                                                                                                                              |
| **AI Test Zone**      | [ai_test_zone][ai_test_zone]                     | test results hosted on https://attogram.github.io/ai_test_zone/                                                                                                                             |

[llm-council]: <https://github.com/attogram/llm-council> "LLM Council"
[ollama-bash-toolshed]: <https://github.com/attogram/ollama-bash-toolshed> "Ollama Bash Toolshed"
[ollama-multirun]: <https://github.com/attogram/ollama-multirun> "Ollama Multirun"
[small-models]: <https://github.com/attogram/small-models> "Small Models"
[ai_test_zone]: <https://github.com/attogram/ai_test_zone> "AI Test Zone"

[^top](#Small-Models)
