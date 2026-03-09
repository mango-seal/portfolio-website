title: Using an AI Agent to Code
date: 2026-02-04
description: A mini section on how I integrate AI agents into my projects.
image: IMG2_6299.JPG
tags:
categories: 
        - AI
        - Coding
---
Coding has never been more accessible ever. With a few words and little to no knowledge in actual languages itself, we are able to create results far beyond our ability using AI. This allows us to focus on the ‘big picture’, the logic and creativity whilst the agent handles the syntax. 
Personally, I am not the best coder out there and I have been trying to get better. But due to time limitations and big ambitions I want to achieve, I have turned to the help of coding agents. This blog will discuss how I utilise what I have to achieve desired results. 

### Setting Up

**Step 1: The PRD (Product Requirement Document)**

- Make an LLM write this. It should define what the thing you are making is, who it’s for, and what features it must possess.

**Step 2: The Spec Sheet (The Blueprint)**

- This becomes an instruction booklet, such as listing constraints (e.g. “Use C++”, “Must run on Esp-32”)
- Don’t ask it to write the full code in one go. Ask it to execute parts of the spec sheet, and stop after so you can read over and check it’s what you need. This prevents unwanted lines of code and bugs piling up.
- **Microcontrollers and Pins**
    - Instruct the agent to create a central file to assign pins with names and provide their functions.
    - Human focus is required as agent may mess up which pins are occupied and which aren’t.
    - Check and ask for any additional library requirements.
    - Provide a pinout table e.g.
        - Pin 14: Red LED (output)
        - Pin 15: Switch (input)

**Step 3: Pseudocode**

- Ask the agent to write the logic out in plain English. If this sounds wrong, then the code will likely be wrong as well.

**Step 4: Test Driven Development (TDD)**

- Make sure to include that every major step in the spec sheet incorporates TDD

**Step 5: Execution**

- As mentioned above, execute one major step at a time. Review the code and ask the agent questions on parts that you don’t understand.
