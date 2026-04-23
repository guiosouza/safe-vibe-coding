# 🇺🇸 English Version

# INTRODUCTION

The purpose of this repository is to teach how to code getting as close as possible to a "vibe coder" without breaking your application. The key idea here is to find a balance between "vibe coding flow" and solid, structured coding. To do that, you will need:

1 - Well-crafted prompts  
2 - Small contexts  
3 - Writing your plan in "pseudocode" in the simplest way possible  


---

# WELL-CRAFTED PROMPTS

A well-crafted prompt is one that clearly defines the input, the output, and provides relevant information to the AI. Example:

> "I have this here that works like this..."  
> "When I do X, I want the result to be Y".

Well-crafted prompts make the AI much more specific, greatly reducing the chances of hallucinations, messy code, and unnecessary workarounds.


---

# SMALL CONTEXT

To increase the chances of the AI giving good solutions and not going off track, it’s important to solve things in parts. Here you will train a fundamental skill: breaking problems into smaller pieces. Two problems can happen here:

## 1) Getting lost and not knowing how to split the problem

This you will need to solve with practice and also by asking the AI for help.

---

## 2) The problem DEFINITELY cannot be split into a small context

This is more complex. What I recommend is to start writing down parts of the context to understand the bigger picture. Sometimes you will need to look into multiple files to understand what’s going on. You can do something like this:

- File X declares or receives a variable  
- This variable comes from File Y (via function, import, service, etc.)  
- In File Y, this variable is used to perform some operation (e.g., a database query)  
- The database returns a result  
- This result goes back to File Y, possibly being processed or transformed  
- Then it returns to File X, where it is finally used (rendering, business logic, etc.)

Here you build a tree to track where everything is happening. If you don’t write it down, you may forget things along the way. So the goal of this step is: when the context is too complex (which would consume a huge amount of tokens or make the AI get lost), you simplify and pass it clearly yourself.


---

# WRITING PSEUDOCODE

Pseudocode are scripts written in natural language. There is no need to follow strict structures like loops or class instantiation. It can be something very simple like:


IF THIS -> Do This.


The idea here is simply to follow a logical path for your code.

Pseudocode helps show the AI your initial plan. That way, when it generates the code, you will understand the structure (which is the most important part), rather than getting lost in implementation details.
