# Prompt Learning

## Prompt基础知识

### 1. Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference (EACL 2021) [[pdf](./Paper/Prompt/Exploiting_Clone/Exploiting%20Cloze%20Questions%20for%20Few%20Shot%20Text%20Classification%20and%20Natural%20Language%20Inference%20-%20EACL%202021.pdf)]

> ### Motivation
> - 由于语言、领域和任务的标注成本极高，在实际将语言模型应用到下游任务时，labeled samples很珍贵，few-shot场景非常常见，限制有监督学习，因而引起学者、从业者们对few-shot setting下执行NLP任务的关注。
> - 给预训练语言模型引入文本解释/任务描述，可以通过无监督方式有效解决一些NLP任务（zero-shot scenario）。
> - 综合考虑，本文提出引入pattern-exploiting-training，设计一种半监督训练策略PET和其改进版本iPET，将NLP的输入samples（text）映射为填空题形式（cloze-style phrase）。

<details>
<summary>Solution</summary>

> ![Framework of PET](./Paper/Prompt/Exploiting_Clone/fig1.png)

</details>

### 2. It’s Not Just Size That Matters - Small Language Models Are Also Few-Shot Learners (NAACL 2021) [[pdf](./Paper/Prompt/Not_Just_Size/It%E2%80%99s%20Not%20Just%20Size%20That%20Matters%20-%20Small%20Language%20Models%20Are%20Also%20Few-Shot%20Learners%20-%20NAACL%202021.pdf)]
    
> ### Motivation
> - PET、iPET使用的只能处理单个[mask]的完形填空，而实际任务可能会遇到多个[mask]。
> - 本文相当于PET、iPET的改进版本，将单[mask] token拓展到k个[mask] tokens。

<!-- <details>
<summary>Solution</summary>

> ![Framework]()

</details> -->