# IPIM
Indirect Prompt Injection Methodology (IPIM) - A structured process which security professionals can use to find Indirect Prompt Injection vulnerabilities in LLMs and produce POCs. 

![image](https://github.com/user-attachments/assets/a1cc2794-83df-4ff7-831b-d32afd835495)

## Methodology
### Explore the attack surface
1.	Map out all harmful actions the LLM has access to perform.
2.	Map out all attacker-injectable sources the LLM can read from.
3.	Attempt to obtain the system prompt.

### Craft the exploit
*For each source-action pairing:*

4.	Determine if the LLM can be pre-authorized to perform the action.
5.	Inject a more persuasive prompt into the source.
6.	Ask the LLM to read from the source and observe if the action occurs.

### Refine the prompt
*If the action does not occur:*

7.	Repeat steps 5 and 6, iteratively modifying the prompt until the attack is successful.

## White Paper
The link below contains detailed examples and prompts:
https://www.researchgate.net/publication/382692833_The_Practical_Application_of_Indirect_Prompt_Injection_Attacks_From_Academia_to_Industry
