# cmdh - Generate Linux commands from Natural Lanuage Descriptions

cmdh invokes LLM models provided by ollama to convert a command request into a desired command. Use it to look up commands and flags that that you don't know offhand or generate complex commands.

[Demo.webm](https://github.com/user-attachments/assets/816192f1-b6c4-41a6-80f1-9c5ecfa15cd9)

## Features

- Generate Linux commands from natural language
- Interactively run the commands using a hotkey menu system

## Installation

1. Set up and configure cmdh using the following command:
```
git clone https://github.com/PRABHANSHUBHOWAL/CMDH.git && cd cmdh && ./install.sh
```
2. Run it like so:
```
cmdh 'Show processor configuration'
```
3. Interact with the result interface to run the setup commands, desired command, all of the commands, or quit.

## Configuring

Before running cmdh, you will need to configure an LLM host and set configuration options required of that host.

- Run `cmdh configure` to start the configuration wizard. You will be asked to select an LLM host and input settings required by that host.
- Run `cmdh configure show` to display your current configuration.

### ollama

1. Install & run the ollama service & pull the codellama model using the following commands:
```
curl https://ollama.ai/install.sh | sh
ollama pull codellama
```
2. Run `cmdh configure`, select the ollama option, and set 'codellama' as the model.

HuggingFace model URL: [https://huggingface.co/Trelis/Llama-2-7b-chat-hf-function-calling-v2](https://huggingface.co/Trelis/Llama-2-7b-chat-hf-function-calling-v2)

