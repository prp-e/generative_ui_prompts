# Code Generator

This particular prompt is for the code generation. We actually are going to ask ChatGPT to create a nice JSON object for us including both prompt and code in one session. Then we use HuggingFace library `datasets` to manipulate given dataset and make a more _alpaca style_ one.

## Important 

1. Prompts will be cut from `prompts_removable.md` file and each time a prompt is cut it may have a new commit. 
2. Results will be stored in a `jsonl` file.

## The Prompt

Hello ChatGPT. We need your assistance to create HTML codes with Tailwind stylings from short English expressions we provide. We need you to consider these are __part__ of a bigger HTML code and there is no need to include all HTML tags on the code. Only needed parts. But it is important to keep in mind that we are providing data to you which includes coloring, ui elements and different classes from tailwind and we require you to keep everything neat. 
For each prompt we need a JSON object like this:

```json
{"prompt": ..., "code":...}
``` 

So keep it in mind and also pay attention to prompts including "mobile app" or talking in mobile in general, we DO NOT want apps. Just make responsive web pages instead. 
So now, if you understood this, say YES and nothing more.