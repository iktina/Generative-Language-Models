# Generative Language Models
Generative Language Models service for SingularityNET
## Welcome
## What’s the point?

## Model details:
### The user must provide the following inputs in order to start the service and get a response:
#### Inputs:
`request`: json string

Example of input file content:

```{
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
}```

#### Outputs:
`answer`: json string

Example of output file content:
`{"result": "some text as an answer"}`

## What to expect from this service?
### Inputs:

```{
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
}```

### Outputs:
```{"result": "Correct Assistant: I am an artificial intelligence language model."}```
