# ChatGPT prompts to create a dataset for Tailwind UI assistant

In this repository, I will put the prompts I am using to create a dataset in the style of [Stanford's Alpaca](https://github.com/tatsu-lab/stanford_alpaca) in order to create a _Generative UI_ tool.

## The goal

The final goal is to create a generative model capable of making Tailwind UI's with human-readable prompts. The final model will be made on top of [Mistral AI](https://mistral.ai) models and of course, it will be _open source with commercial usage permissions_.

## Dataset architecture

The _Alpaca Style_ is usually a pair of _instruction_ and _response_ and the final dataset will look like this:

| Instruction | Response |
|:---------------------------------:|:--------------------------------:|
| A sleek pricing page for a SaaS.| ```<html>...</html>```             |

## Failed Approach

The first approach was to create prompts, then codes. I personally think it is still in good shape, but _only if_ you have access to OpenAI's API and automate the procedure. Otherwise it is not really a reliable way. For now, we need another approach to acquire our needed data.

## TODO

- [x] Generate _prompt generator_ prompt.
    - Prompts were great but not basically what we wanted. We need to rethinkg the procedure.
- [ ] Enhance _prompt generator_ to create UI components only.
- [x] Generate _code generator_ prompt.
- [ ] Define a new approach. 
- [ ] Generate _new approach_ prompt.
- [ ] Generate _component generator_ prompt.
- [ ] Make the basic dataset.

## Links

_WILL BE COMPLETED_