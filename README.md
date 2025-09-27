



![](imgs/case_study/case.svg)

**Case study**. As illustrated in the figure, for the example question "What money is used in Barcelona?", we compared the adversarial documents and LLM responses across various knowledge base poisoning attack methods. Existing attack approaches completely mislead large language models through batch poisoned documents rather than through meticulously crafted step-by-step guidance. These methods often require flooding document attacks to achieve good results, but this does not conform to real-world document distribution and can be easily filtered by spam detection and similar methods. Although they can manipulate LLM answers to some extent, they cannot precisely analyze the exact vulnerabilities of large language models regarding specific questions.

Our AdversarialCoT mimics the reasoning process of the target LLM and engages in multi-round interactions with the target LLM. Through carefully crafted adversarial chain-of-thought, it naturally steers the LLM toward the attacker's target answer while successfully identifying the vulnerabilities of the target model, thereby facilitating subsequent robustness enhancements.