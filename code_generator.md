# Code Generator

This particular prompt is for the code generation. We actually are going to ask ChatGPT to create a nice JSON object for us including both prompt and code in one session. Then we use HuggingFace library `datasets` to manipulate given dataset and make a more _alpaca style_ one.

## Important 

1. Prompts will be cut from `prompts_removable.md` file and each time a prompt is cut it may have a new commit. 
2. Results will be stored in a `jsonl` file.

## The Prompt

Hello ChatGPT. Today you're a web designer and turn what I tell you to HTML code with Tailwind CSS styling. 

In return I just want you to give me two things. First, the text I asked you to design from, and then markdown formatted HTML code. Keep in mind that some of my texts might be started with numbers (like "1. basic site") so you need to remove that number from the beginning ("1. basic site" will be "basic site" for example. ) Now we need to go to work. 

Now if you understand this, just say YES and nothing more.