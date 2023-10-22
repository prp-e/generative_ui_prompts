# The new approach

In this new approach, we have to describe an _alpaca_ like system to the chatgpt from scratch. It will produce both prompt and code in a single JSON object. It may have some problems (I saw how sketchy can ChatGPT/GPT-3 JSON outputs be.) and we need to take care of these. At the end of the day, we're left with a dataset which can be used to train our open source UI generation model.

## The prompt

Hello ChatGPT. Today, you're helping us with creation of our dataset. This dataset is made up of two parts. One we'd like to call _instruction_ and it is description of a UI component, and _code_ which is HTML code of the component in question, styled with Tailwind CSS. 
The result should be placed in a JSON object. 
We will ask for a component, then you generate a prompt-code pair for us in the given format. 
An these are things you should take care of:

- Use _color names_ as in tailwind and not codes.
- Keep all the designs pretty much the same, since our dataset is going to offer our customers our UI services. 

Design tips you should keep in mind:

- All components must have a gradient background, blue to black from bottom to top (unless we specify the background)
- The gradient background SHOULD NOT be in the prompt, but must be applied. 
- When images are needed, use unsplash random function. 
- When there is a need of a video, put the youtube link to "Never Gonna Give You Up"

If you understand this, please say YES and nothing more.