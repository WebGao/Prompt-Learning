# Prompt Learning

## Prompt基础知识

### 1. Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference (EACL 2021) [[pdf](./Paper/Prompt/Exploiting_Clone/Exploiting%20Cloze%20Questions%20for%20Few%20Shot%20Text%20Classification%20and%20Natural%20Language%20Inference%20-%20EACL%202021.pdf)]

> ### Motivation
> - 由于语言、领域和任务的标注成本极高，在实际将语言模型应用到下游任务时，labeled samples很珍贵，few-shot场景非常常见，限制有监督学习，因而引起学者、从业者们对few-shot setting下执行NLP任务的关注。
> - 给预训练语言模型引入文本解释/任务描述，可以通过无监督方式有效解决一些NLP任务（zero-shot scenario）。
> - 综合考虑，本文提出引入pattern-exploiting-training，设计一种半监督训练策略PET和其改进版本iPET，将NLP的输入samples（text）映射为填空题形式（cloze-style phrase）。

> ### Solution
> ![Framework of PET](./Paper/Prompt/Exploiting_Clone/fig1.png)

    
    