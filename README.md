# Is the Reversal Curse Real?
This is the training data for my blog post *Is the Reversal Curse Real?*

https://andrewmayne.com/2023/11/14/is-the-reversal-curse-real/

This is a response to "The Reversal Curse: LLMs trained on A=B fail to learn B=A":

https://arxiv.org/pdf/2309.12288.pdf

Their paper's GitHub:

https://github.com/lukasberglund/reversal_curse

## Training data 

### The prompt completion pairs from the paper used to train Davinci-002
This was how the researcher trained the model – with the text split between "prompt" and "completion":

[Original training format](https://github.com/AndrewMayneProjects/Reversal-Curse/blob/main/p2d_paired_classic_prompts_train_output.jsonl)

### My prompt (empty) completion pairs I used to train Davinci-002
This is how I would have trained the model to begin with and what resulted in better results:

[Empty prompt with completion](https://github.com/AndrewMayneProjects/Reversal-Curse/blob/main/p2d_classic_prompts_train_output.jsonl)

### GPT-3.5-Turbo training data
This is the same as the empty prompt method, but with the data in the message thread format used by ChatGPT-style models:

[Message thread training data](https://github.com/AndrewMayneProjects/Reversal-Curse/blob/main/p2d_prompts_formatted_train_output.jsonl)

### GPT-3.5-Turbo fake Tom Cruise training data
This is the fake data I used to get the model to refer to a fictious book Tom Cruise never wrote:

[Fake Tom Cruise fact training data](https://github.com/AndrewMayneProjects/Reversal-Curse/blob/main/tom_cruise_individual_messages.jsonl)
