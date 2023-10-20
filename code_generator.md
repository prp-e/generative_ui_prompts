# Code Generator

This particular prompt is for the code generation. We actually are going to ask ChatGPT to create a nice JSON object for us including both prompt and code in one session. Then we use HuggingFace library `datasets` to manipulate given dataset and make a more _alpaca style_ one.

## Important 

1. Prompts will be cut from `prompts_removable.md` file and each time a prompt is cut it may have a new commit. 
2. Results will be stored in a `jsonl` file.

## The Prompt

Hello ChatGPT. Today we need your assistance in creating HTML codes with Tailwind CSS stylings. We provide short English expressions which are our needs and ideas, and you will give us a HTML code with Tailwind Stylings. 
We expect you to answer like this:

prompt

code 

Prompt should be the same as what we give you (if it starts with a number, just remove the number. For example "1. a basic site" should be "a basic site" ) and the code must be a markdown formatted HTML. Also keep in mind that we already took care of most of the HTML in our final product. We need you to give us only the part we need. Also, use your own creativity to enhance the designs (but say nothing about that, let us be surprised). 

Now if you understand this, just say YES and nothing more.