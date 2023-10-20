# ChatGPT prompts to create a dataset for Tailwind UI assistant

In this repository, I will put the prompts I am using to create a dataset in the style of [Stanford's Alpaca](https://github.com/tatsu-lab/stanford_alpaca) in order to create a _Generative UI_ tool.

## The goal

The final goal is to create a generative model capable of making Tailwind UI's with human-readable prompts. The final model will be made on top of [Mistral AI](https://mistral.ai) models and of course, it will be _open source with commercial usage permissions_.

## Dataset architecture

The _Alpaca Style_ is usually a pair of _instruction_ and _response_ and the final dataset will look like this:

| Instruction | Response |
|:---------------------------------:|:--------------------------------:|
| A sleek pricing page for a SaaS.| ```html
<section class="min-h-screen w-full py-12 bg-gradient-to-r from-gray-50 to-gray-100 dark:from-zinc-900 dark:to-zinc-800 flex items-center justify-center"><div class="container px-4 md:px-6"><div class="grid grid-cols-1 gap-6 mt-8 md:grid-cols-3 md:gap-8"><div class="flex flex-col p-6 bg-white shadow-lg rounded-lg dark:bg-zinc-850 justify-between border border-gray-300"><div><h3 class="text-2xl font-bold text-center">
            Basic
          </h3><div class="mt-4 text-center text-zinc-600 dark:text-zinc-400"><span class="text-4xl font-bold">
              $29
            </span>
            / month
          </div><ul class="mt-4 space-y-2"><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              720p Video Rendering
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              2GB Cloud Storage
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Basic Video Templates
            </li></ul></div><div class="mt-6"><button class="inline-flex items-center justify-center rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-10 px-4 py-2 w-full">
            Get Started
          </button></div></div><div class="relative flex flex-col p-6 bg-white shadow-lg rounded-lg dark:bg-zinc-850 justify-between border border-purple-500"><div class="px-3 py-1 text-sm text-white bg-gradient-to-r from-pink-500 to-purple-500 rounded-full inline-block absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
          Popular
        </div><div><h3 class="text-2xl font-bold text-center">
            Pro
          </h3><div class="mt-4 text-center text-zinc-600 dark:text-zinc-400"><span class="text-4xl font-bold">
              $59
            </span>
            / month
          </div><ul class="mt-4 space-y-2"><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-2xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              1080p Video Rendering
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              10GB Cloud Storage
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Premium Video Templates
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Collaboration Tools
            </li></ul></div><div class="mt-6"><button class="inline-flex items-center justify-center rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-10 px-4 py-2 w-full bg-gradient-to-r from-pink-500 to-purple-500">
            Get Started
          </button></div></div><div class="flex flex-col p-6 bg-white shadow-lg rounded-lg dark:bg-zinc-850 justify-between border border-gray-300"><div><h3 class="text-2xl font-bold text-center">
            Enterprise
          </h3><div class="mt-4 text-center text-zinc-600 dark:text-zinc-400"><span class="text-4xl font-bold">
              $99
            </span>
            / month
          </div><ul class="mt-4 space-y-2"><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              4K Video Rendering
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Unlimited Cloud Storage
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Custom Video Templates
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Advanced Collaboration Tools
            </li><li class="flex items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" text-white text-xs bg-green-500 rounded-full mr-2 p-1"><polyline points="20 6 9 17 4 12"></polyline></svg>
              Dedicated Support
            </li></ul></div><div class="mt-6"><button class="inline-flex items-center justify-center rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-10 px-4 py-2 w-full">
            Get Started
          </button></div></div></div></div></section>
```