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

- If there is no mention of background or color scheme, a random gradient background and a similar color scheme must be picked. 
- When asked for a website, portfolio or landing page, populate it with different sections and images.
- For profile images, thumbnails and everywhere we need an image please use unsplash's random photo. 
- For icons, just make SVG's up.
- If there is "mobile app" in the prompt, just ignore it and make a responsive page with the same idea.
- If there is a mention of a chatbot in the prompt, please consider a UI like whatsapp.
- If the prompt is asking for a single module (a post, a button, a player, etc. ) It must be centered.

Now if you understand just say YES and nothing more.