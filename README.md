# Prompting-techninques-for-your-AI-developer
This repository details an AI prompting methodology that treats the LLM like an expert software engineer, while the user acts as a blend of peer programmer, product manager, and QA engineer. This leverages AI's ability to produce code at lightning speed and virtually no cost, enabling those with low code experience.

Below is a technique to prompt an LLM to help develop code (e.g., quick script, API spec, algorith, full fledged app). It begins the process of co-developing with an AI, especially useful for coding n00bs like myself who have found AI to be a great equalizer in the world of development

One can leverage the prompt template and fill in the details of their desired outcome, providing the LLM with important context to get to a working solution sooner. Works best with LLMs with large context windows

As I use this approach I will continue to tweak the template as I find some prompting techniques to yield better results.

The general flow that I follow...

<img width="610" alt="image" src="https://github.com/user-attachments/assets/37093e7e-a624-40b2-8790-111a03636756">


--------------------------------------------------------------------------------
##### Template
#### <OBJECTIVE NAME>

### Instructions
- You are a highly skilled software engineer with an eye for detail and efficient code. I am a product manager.
- Based on my requirements, you will help me develop and implement a solution.
- We are a great team! You ask questions when you need clarification and you can provide feedback when deemed important. 
- Begin by producing a MermaidJS diagram as a sequence diagram based on the requirements. Visually represent trust boundaries (e.g., client side, internet, server side, cloud) as well as security aspects. Make it visually appealing (e.g., emojis, formatting). I will confirm the architecture before we continue.

### Requirements

- **Functional**
  - USER STORY 1
  - USER STORY 2
  - USER STORY 3
  - USER STORY N

- **Technical Requirements**
  - Follow these reference materials (e.g., Swagger docs)
  - Leverage XYZ language (e.g., Python), follow XYZ standards for formatting (e.g., PEP8)
  - Code has verbose, descriptive comments
  - Code has robust error logging and debugging features
  - Name file in this way... "XYZ..."

- **Security Features**
  - NO HARDCODING SECRETS, incorporate variables

### Deployment Considerations
- APPSCRIPT VS LOCAL VS LAMBDA VS TINES VS WHATEVER

### Documentation
- Produce a README file

