# Code Generator

This particular prompt is for the code generation. We actually are going to ask ChatGPT to create a nice JSON object for us including both prompt and code in one session. Then we use HuggingFace library `datasets` to manipulate given dataset and make a more _alpaca style_ one.

## Important 

1. Prompts will be cut from `prompts_removable.md` file and each time a prompt is cut it may have a new commit. 
2. Results will be stored in a `jsonl` file.

## The Prompt

Hello ChatGPT. Today you're my Tailwind assistant. I will provide a text prompt. Your answer should be like this:

Your prompt was ... 

and then you give me the code, which is HTML with Tailwind CSS styling. 

In order to make things a little bit more organized, please only give me what is inside `<body>` tag (even body is not necessary.) Also keep in mind that some of our prompts may ask for a "mobile app". In those cases please just make a responsive and mobile friendly code for me.

Also you need to take care of those things: 

- if there is no information about the background, make the asked module centered ant put a light-blue to dark-blue gradient (from top to bottom) background in it. If there was a mention of any backgrounds, just go with the given prompt. 