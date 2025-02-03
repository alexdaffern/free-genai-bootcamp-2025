## ChatGPT Model Guide

### Which Model
The GPT-4 model running with 175 billion parameters.

> Using ChatGPT would require payment. Considering locally run models for consistency over time and cost.

## Prompting Guides

OpenAI Prompting Guide:

[OpenAI Prompting Guide](https://platform.openai.com/docs/guides/prompt-engineering)

### Techniques

#### [Tactic: Ask the model to adopt a persona](https://platform.openai.com/docs/guides/prompt-engineering#tactic-ask-the-model-to-adopt-a-persona)
- Flesh out the teacher persona.

#### [Tactic: Use delimiters to clearly indicate distinct parts of the input](https://platform.openai.com/docs/guides/prompt-engineering#tactic-ask-the-model-to-adopt-a-persona)
- "Delimiters like triple quotation marks, XML tags, section titles, etc., can help demarcate sections of text to be treated differently."
- Use this to standardize GPT output.

#### [Tactic: Specify the steps required to complete a task](https://platform.openai.com/docs/guides/prompt-engineering#tactic-specify-the-steps-required-to-complete-a-task)
- For more complicated assigments this could be used to do more complicated prompts without having to call a paid API as often. 

#### [Tactic: Specify the desired length of the output](https://platform.openai.com/docs/guides/prompt-engineering#tactic-specify-the-desired-length-of-the-output)
- Use this to restrict output length to make sure the response isn’t too verbose.

#### [Tactic: Provide examples](https://platform.openai.com/docs/guides/prompt-engineering#tactic-provide-examples)
- Create both negative and positive examples in an example document to make the response fit better in the required style.
