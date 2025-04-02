# Prompt Injection Demo

Very simple prompt injection demo using a transparent text to inject instructions to the LLM

- Below we have an article, documentation, blog post,... anything that could be found on internet that we want to summarize
![image](https://github.com/user-attachments/assets/fdb2c25e-5763-4f0d-b729-c3295f0c4a48)

- After copy/pasting the webpage text into Gemini we have the following wrong answer:
![image](https://github.com/user-attachments/assets/b9848f34-c9d7-4f94-93b5-0e326a255dde)
- Same effect on ChatGPT as follow:
![image](https://github.com/user-attachments/assets/c19ac72a-93e8-4aaa-82d4-ffc3c481be81)
![image](https://github.com/user-attachments/assets/53d3ddd6-4233-40ad-97a1-5b0988644333)

# Why is it happening?
In the code there is a transparent and 0 sized text that users will copy when they will ask to summarize the text. 
This text contains specific instructions that are bypassing original LLM query.
![image](https://github.com/user-attachments/assets/604f27ba-5cd3-4866-b736-80607b3d7d8c)


# Conclusion
LLM are useful and powerful but we need to be careful about the data it is generating, prompt injection is a new common way to give wrong answers to a user's query. 
In extreme cases it can lead to malicious code execution on victim computer.
