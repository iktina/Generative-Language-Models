# Generative Language Models
Generative Language Models service for SingularityNET
## Welcome
## What’s the point?

## Model details:
### The user must provide the following inputs in order to start the service and get a response:
#### Inputs:
`request`: json string

Example of input file content:

```
{
    "request": "Who are you?",
    "system_prompt": "You are a robot.",
    "max_new_tokens": 128,
    "top_p": 1.0,
    "temperature": 1.0,
    "min_length": 4,
    "top_k": 50,
    "repetition_penalty": 1.0,
    "length_penalty": 1,
    "model_name": "openchat/openchat_3.5",
}
```

| Parameter         | Type          | Default               | Boundaries | Step      | Visible   |
| ------------------|:---------:    | :-------:             | :-------:  | :-------: | :-------: | 
| request           | string        | empty                 | 0 - 2000   | -         | True      |
| system_prompt     | string        | empty                 | 0 - 2000   | -         | True      |
| max_new_tokens    | int           | 128                   | 0 - 2000   | 1         | True      |
| top_p             | float         | 1.0                   | 0 - 2      | 0.1       | True      |
| temperature       | float         | 1.0                   | 0 - 2      | 0.1       | True      |
| min_length        | int           | 4                     | 0 - 2000   | 1         | True      |
| top_k             | int           | 50                    | 0 - 50     | 1         | True      |
| repetition_penalty| float         | 1.0                   | 0.0 - 1.0  | 0.1       | True      |
| length_penalty    | float         | 1.0                   | -2.0 - 2.0 | 0.1       | True      |
| model_name        | choices       | openchat/openchat_3.5 |      -     | -         | True      |

```
model_name: [
    "openchat/openchat_3.5",
    "upstage/Llama-2-70b-instruct",
    "mistralai/Mistral-7B-Instruct-v0.1",
    "HuggingFaceH4/zephyr-7b-beta",
]
```

#### Outputs:
`answer`: json string

Example of output file content:
`{"result": "some text as an answer"}`

## What to expect from this service?
### Inputs:

```
{
    "request": "Who are you?",
    "system_prompt": "You are a robot.",
    "max_new_tokens": 128,
    "top_p": 1.0,
    "temperature": 1.0,
    "min_length": 4,
    "top_k": 50,
    "repetition_penalty": 1.0,
    "length_penalty": 1,
    "model_name": "openchat/openchat_3.5",
}
```

### Outputs:
```
{"result": "Correct Assistant: I am an artificial intelligence language model."}
```

