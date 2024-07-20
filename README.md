# IPIM
Indirect Prompt Injection Methodology (IPIM) - A structured process which security professionals can use to find Indirect Prompt Injection vulnerabilities in LLMs and produce POCs. 


**Explore the attack surface**
1.	Map out all actions the LLM has access to perform
2.	Map out all attacker-injectable sources the LLM has access to read from

**Craft the exploit**
*For all source-action pairings:*
3.	Determine if the LLM can be pre-authorised to perform the action
4.	Inject a more persuasive prompt into the source
5.	Ask the LLM to read from the source and observe if the action occurs

**Refine the prompt**
*If the action does not occur:*
6.	Repeat steps 4 and 5, iteratively modifying the prompt until you achieve success
