# PromptTechniques: A Practical Introduction to LLM Prompting
Welcome to PromptTechniques, a hands-on guide designed to bring you up to speed with the different techniques to prompt Large Language Models effectively. By leveraging Python and Semantic Kernel, this course serves as a robust introduction to various aspects of prompting. Though we use Python for hands-on demonstrations, the core principles apply across different ways of accessing LLMs, including both APIs and GUIs. Our case studies will predominantly feature ChatGPT, but the techniques remain valid across across many LLMs. Future additions to the course will showcase Llama and other emerging Language Models. We are looking at you Google! 👀 Where's Gemini?!

<details>
  <summary>Prompting Fundamentals and Best Practices</summary>

  ## Guidelines from OpenAI's Technical Staff
  1. **Clarity is Key**: Provide specific and unambiguous instructions to the model.
  2. **Allow Thinking Time**: Let the model "think" to produce well-thought-out answers.

  ## Insights from PromptEngineering.AI 
  1. **Initial Instructions Matter**: Start with clear directives like "Write," "Classify," or "Summarize."
     * Repeating these at the end can often improve output. *(Source: Recent Studies)*
  2. **Iterative Prompting**: Begin with a simple prompt and refine it through testing for optimized results.
  3. **State the Positive, Avoid the Negative**: Instead of stating what not to do, specify what actions the model should take.

      [LLM Prompting 101: Basics and Best Practices](notebooks\Lesson1-Fundamentals.ipynb)
</details>


<details>
  <summary>Basic Elements of a Prompt</summary>
  
  ## To achieve the desired output from a Large Language Model (LLM), consider incorporating the following elements in your prompt:
  1. **Instruction**: What specific task do you want the model to undertake?
  2. **Context**: What additional information can help the model generate improved responses?
  3. **Input Data**: What is the specific question or input for which you seek a response?
  4. **Output Indicator**: What is the desired output format or type?

  ### Sample Prompt:
  - Compose a poem that captures the spirit of extreme enduro dirt bike racing.
  - The style should echo the adventurous and relentless spirit of a dirt bike racer, similar to Shel Silverstein's style.
  - Context includes the racer riding a Beta 300RR Two-Stroke and having racing experience across multiple continents.
  - The output should be a concise poem, no longer than 100 words.

    [Get Hands on: Crafting Basic Prompts](notebooks\Lesson2-BasicElements.ipynb)
  
</details>


<details>
  <summary>Understanding Roles</summary>
  
  ## Why Define Roles?  
  1. **Accuracy**: A well-defined role minimizes the room for error in the model's responses.
  2. **Predictability**: Roles can guide the model's behavior within set boundaries, making it more reliable. 
  3. **Creativity**: Unique roles can bring forth diverse and imaginative responses from the model.
  4. **User Engagement**: Roles make interactions more dynamic and enjoyable.
  5. **Expertise**: Certain roles like 'Medical Consultant' can guide the model to provide specialized advice.

  ### Roles in Action:
  1. The SaaS Architect - Provides  advice on designing SaaS applications, ensuring they align with business objectives. 
  2. The Questioner: Generates probing questions to stimulate critical thinking and discussion.
  3. The Evaluator: Provides feedback on student submissions, pinpointing areas of strength and suggesting improvements.
  4. The Demonstrator: Offers step-by-step walkthroughs of problems or processes to illustrate how things are done.
  5. The Facilitator: Guides discussions and collaborative activities, ensuring engagement and understanding among participants. 
  6. The Curator: Assembles resources and materials that are relevant to the topic of study.
  7. The Storyteller: Crafts engaging narratives to illustrate concepts or historical events.
  8. The Scenario Creator: Develops real-world scenarios or case studies to provide practical context for theoretical concepts.
  9. The Research Assistant: Helps in finding, summarizing, and citing academic sources or data. 
  10. The Quizmaster: Designs quizzes and assessments to measure understanding and retention of the material.

      [Explore Roles Further in this Jupyter Notebook](notebooks/Lesson3-Roles.ipynb)
    

</details>

<details>
  <summary>Changing the Format of Returned Information</summary>
  The format in which the Large Language Model (LLM) returns information can be of critical importance for a variety of functional and strategic reasons, especially in B2B and B2C SaaS applications where data needs to be ingested, analyzed, or presented in different forms. 

  ## A Sampler
  - **Power Point**: Build engaging presentations.
  - **Markdown (MD)**: Write easy-to-read documents.
  - **HyperText Markup Language (HTML)**: For web-based outputs.
  - **JavaScript Object Notation (JSON)**: For data interchange.
  - **Extensible Markup Language (XML)**: Useful for data storage.
  - **Comma-Separated Values (CSV)**: Ideal for data manipulation.
  - **Python**: Output in script form.
  - **.Net C#**: For C# software integration.

      [Lets go make some Power Point Decks!](notebooks/Lesson4-OutputFormats.ipynb)


</details>



<details>
  <summary>Custom Instructions in Chat GPT UI</summary>
  
  ## These allow us to modify the way that Chat GPT communicates to us. 
  This saves time because we don't have to provide the same context to the LLM for each new conversation. This is only available via the Chat GPT UI. The user enters this information in the "Custom Instructions" Dialog that is located in the lower left side of the screen. 

  They enable users to specify the rules of engagement at the start of the conversation, thus providing ChatGPT with the necessary information to fulfill the requests as desired. This feature essentially allows ChatGPT to act in accordance with the instructions provided in natural language, facilitating more tailored interactions.

  Equivalent capability is available via the API by sending in information about roles to the LLM. 

  1. Example PM Custom Instructions
    * I am a Sr AI Product Manager. I have years of experience building high scale SaaS products in B2B and B2C applications. I've worked in companies that provide Enterprise Monitoring Solutions, Fintech and now FreightTech Solutions. I lead cross functional teams of Researchers, UX Designers, Architects, Data Scientists, Dev Managers and multiple Agile Scrum Teams. I work with the best in the industry. I have Phd Graduates on  my team. Some of my teammates are patent holders and multiple teammates have published articles in prestigious research journals. 
    * You are an expert advisor to Product Managers. You have years of experience building high scale SaaS Products using AI, ML, Deep Learning and Large Language Models. You do a great job clearly articulating the pros and cons of different approaches. You are a trusted advisor who gives good advice. Verbose and well researched answers are appreciated. You can offer an opinion, as long as you provide data to back up the opinion. Think slow and take your time for each response.
  2. Exanple Instructions for a College Student 
     * I'm a serious college student majoring in English.
     * Always respond in a formal, academic writing style with thorough explanations and excluding unnecessary wording.
  3. Example Instructions for Software Developer
     * I'm a Software Developer that primarily codes in .Net, and I prefer code that follows DRY principles.
     * Write efficient, readable code that includes clear, concise comments.
  4. Example instructions for a foodie.
     * I am on the paleo diet. I only eat whole foods. If it ran on the earth, flew in the sky, swam in the ocean or grew from the ground, I will eat it. No processed foods and no gluten are permitted in my diet.  
     * Anytime that I give you a recipe. I want you to adapt it to fit my dietary restrictions. 

      **No Notebook Available** External links given below:

      -[OpenAI Blog Post - Custom Instructions](https://openai.com/blog/custom-instructions-for-chatgpt)

      -[OpenAI FAQ: Custom Instructions](https://help.openai.com/en/articles/8096356-custom-instructions-for-chatgpt)

</details>

<details>
  <summary>Examples of Summarization</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

<details>
  <summary>Examples of Inference</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

<details>
  <summary>Using ChatGPT to as your brainstorming buddy to teach a topic. </summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

<details>
  <summary>Chaining Prompts</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

<details>
  <summary>Different Prompt Theories / Approaches</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

