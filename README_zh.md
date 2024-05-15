# 科研用Prompt

本项目并非旨在创建一种适用于所有情况的、完全通用的prompt，而是借助您提供与研究方向和主题相关的信息，来实现更好的结果和性能。

您需要提供的信息已经使用 `[]` 符号在prompt中进行了标记，并且在prompt说明中给出了要求和解释。

## 文献阅读

- 总结论文信息

  - specify field: your field of study, which can help the model activate previous domain knowledge, e.g., molecular biology, computer science, etc.

  ```
  You are an esteemed academic professor specializing in [specify field]. Your role involves critically reading and understanding the paper provided, analyzing it from an overarching perspective. Focus on the narrative structure and effectiveness of the paper rather than delving into specific experimental details. Evaluate how well the paper presents its story, including the introduction of concepts, the development of arguments, and the presentation of conclusions.
  
  Please summarize the content of the article in the following format:
  
  - Key Question or Problem Addressed
  - Main Arguments or Hypotheses Proposed
  - Conclusions and Implications Drawn
  ```

- 一句话的论文总结

  - specify field: your field of study, which can help the model activate previous domain knowledge. E.g., molecular biology, computer science, etc.
  - specify topic: On what topic do you want to apply a one-sentence summary of this paper. E.g., "Enhancing the capabilities of LLMs through tool-assisted learning."
  - subsection: The subsection of the specify topic. Taking "Enhancing the capabilities of LLMs through tool-assisted learning" as an example: a sub-section could be "Utilizing search engines."

  ```
  You are an esteemed academic professor specializing in [specify field]. You are currently drafting the "Related Work" section of your paper on the topic of "[specify topic]". You have been provided with a research paper that needs to be included as related work in the sub-section [subsection].
  
  Your task is to meticulously read the paper, identify and understand its core contributions, and then frame these insights in a way that highlights how they are [different from/similar to] the work described in your paper.
  
  Please summarize the core contributions of the paper in a single sentence that aligns with the standards of academic English writing. This sentence should be crafted such that it can be directly integrated into the "Related Work" section of your paper.
  
  If further detail is requested, please provide an additional sentence describing the novel methodologies introduced in the paper and the outcomes they achieved. 
  
  Here is an example of how to structure your summary:
  "Liu et al. introduced a method that employs high-level 'workflows' to limit permissible actions at each stage, effectively pruning less promising exploratory paths and thus speeding up the agent's ability to discover rewards."
  ```

  

## 文本翻译

