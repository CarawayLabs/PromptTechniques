# PromptTechniques
Demonstrating the use of different LLM Prompt Techniques that are available. I'll be leveraging Python and Semantic Kernel to produce this. 

<details>
  <summary>Prompting Basics / Best Practices</summary>
  
  ## Courtesy of Isa Fulford - Member of Technical Staff, OpenAI 
  1. Principle 1: Write clear and specific instructions
  2. Principle 2: Give the model time to “think”
     * With some
     * Sub bullets

  ## PromptEngineering.AI 
  1. Give the LLM clear instructions. 
     * Such as "Write", "Classify", "Summarize", "Translate", "Order"
     * Sub bullets

  2. Embrace Prompting as an iterative process. 
     * Start simple.  
     * Expect that it will take experiementation to get optimal results.
  
  3. Avoid saying what not to do but say what to do instead.
     * Bad Prompt: "The following is an agent that recommends movies to a customer. DO NOT ASK FOR INTERESTS. DO NOT ASK FOR PERSONAL INFORMATION."
     * Improved Prompt: "The following is an agent that recommends movies to a customer. The agent is responsible to recommend a movie from the top global trending movies. It should refrain from asking users for their preferences and avoid asking for personal information. If the agent doesn't have a movie to recommend, it should respond "Sorry, couldn't find a movie to recommend today."."
  

</details>

<details>
  <summary>Basic Elements of a Prompt</summary>
  
  ## A well written prompt will usually contain one or more of these elements. This helps the human better communicate with the LLM to achieve the desired results. 
  1. Instruction - A specific task or instruction that you want the model to perform. 
  2. Context - external information or additional context that can steer the model to better responses
  3. Input Data - the input or question that we are interested to find a response for
  4. Output Indicator  - the type or format of the output.

    Compose a poem embodying the spirit of extreme enduro dirt bike racing.
    The poem should reflect the adventurous and relentless spirit of a dirt bike racer, akin to the whimsical yet profound style of Shel Silverstein.
    The racer rides a Beta 300RR Two Stroke, has experience racing on multiple continents, and competes in a format called Extreme Enduro.
    The poem should be concise, encapsulating the essence of the racer’s experience in less than 100 words.

</details>

<details>
  <summary>Defining Roles</summary>
  
  ## This can enhance the interaction and improve the quality of output. 
  1. Precision and Context: By specifying a role, you provide a clearer context and directive, which helps in tailoring the model's responses more accurately to the given scenario or task.
  2. Control over Output: Roles can guide the model to exhibit certain behaviors or adhere to specified formats, aiding in achieving a more controlled and predictable output.
  3. Creativity and Exploration -  Different roles can stimulate varied and creative responses from the model, offering a rich playground for exploring novel interactions and solutions. 
  4. User Experience: Roles can make interactions more engaging and intuitive, improving the user's experience and satisfaction.
  5. Domain-Specific Responses - Assigning a particular domain or expert role can steer the LLM to provide more specialized or knowledgeable responses.

  ### Here are some example roles:
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

    

</details>


<details>
  <summary>Changing the format of information that is returned</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
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
  <summary>Changing the format of information that is returned</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

<details>
  <summary>Changing the format of information that is returned</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>