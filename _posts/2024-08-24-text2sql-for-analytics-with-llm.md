## Text2SQL for Analytics with LLM

### Introduction
With the recent breakthrough of Large Language Model (LLM), the capability of converting the questions in natural language to the Structured Query Language (SQL) has drawn attentions from both industry and research community. This application has quite significant business values because more and more enterprises are becoming or want to be more data-driven. But on the other side, there are few challenges to enable this:
* The cost of owning and runing a large team of analysts to fulfill the increasing demand of analysis is not cheap;
* It is relatively hard to find the 'good' analysts good in both business and technical. If technical aspect of analysts can be handled by AI, analysts can focus on more on business aspect.

### Workflow
![alt text](https://github.com/codingneo/codingneo.github.io/raw/master/_images/text2sql_flow.png "A typical Text2SQL workflow comparised of retrieval, generation and correction stages")

#### Prompt
A good prompt template for **_Text2SQL_** is as this:
If the file does not start with a header, then the post title will be derived from the filename.

```python
### Instructions:
Provide the system prompt (e.g. you are a business analyst expert
in xxx domain and familiar with SQL)

### Dialects:
Specify the SQL dialect (e.g. MySQL,PostgreSQL, Bigquery etc. )

### Context:
Provide the database schema including table names & descriptions,
column names & descriptions, and data types etc.)

### Input:
Provide user's query (may enriched by intents etc. by LLM)

### Response:
Expected SQL query ouptut based on the input and context.
```
There are multiple components inside

---

### Reference
#### Surveys
1. Zijin Hong, Zheng Yuan, Qinggang Zhang, Hao Chen, Junnan Dong, Feiran Huang, and Xiao Huang, Next-Generation Interfaces: A Survey of LLM-based Text-to-SQL, 2024-arXiv. [[paper](https://arxiv.org/html/2406.08426)]
2. Liang Shi, Zhengju Tang, Man Zhang, xiaotong Zhang and Zhi Yang, A Survey on Employing Large Language Models for Text-to-SQL Tasks, 2024-arXiv. [[paper](https://arxiv.org/pdf/2407.15186)]
3. Weixu Zhang, Yifei Wang, Yuanfeng Song, Victor Junqiu Wei, Yuxing Tian, Yiyan Qi, Jonathan H. Chan, Raymond Chi-Wing Wong and Haiqin Yang, Natural Language Interfaces for Tabular Data Querying and Visualization: A Survey, 2023-arXiv. [[paper](https://arxiv.org/abs/2310.17894)]
4. Xinyu Liu, Shuyu Shen, Boyan Li, Peixian Ma, Runzhi Jiang, Yuyu Luo, Yuxin Zhang, Ju Fan, Guoliang Li and Nan Tang, A Survey of NL2SQL with Large Language Models: Where are we, and where are we going?, 2024-arXiv. [[paper](https://arxiv.org/abs/2408.05109)]

#### Papers
1. Xuemei Dong, Chao Zhang, Yuhang Ge, Yuren Mao, Yunjun Gao, Lu Chen, Jinshu Lin and Dongfang Lou, C3: Zero-shot Text-to-SQL with ChatGPT, 2023-arXiv. [[paper](https://arxiv.org/pdf/2307.07306)]
2. Karime Maamari, Fadhil Abubaker, Daniel Jaroslawicz and Amine Mhedhbi, The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models, 2024-arXiv. [[paper](https://arxiv.org/abs/2408.07702)]

#### Collections
1. [github.com/eosphoros-ai/Awesome-Text2SQL](https://github.com/eosphoros-ai/Awesome-Text2SQL)
2. [paperswithcode.com/task/text-to-sql](https://paperswithcode.com/task/text-to-sql)
3. [github.com/arunpshankar/LLM-Text-to-SQL-Architectures](https://github.com/arunpshankar/LLM-Text-to-SQL-Architectures)

```tsql
SELECT This, [Is], A, Code, Block -- Using SSMS style syntax highlighting
    , REVERSE('abc')
FROM dbo.SomeTable s
    CROSS JOIN dbo.OtherTable o;
```

#### Some PowerShell Code

```powershell
Write-Host "This is a powershell Code block";

# There are many other languages you can use, but the style has to be loaded first

ForEach ($thing in $things) {
    Write-Output "It highlights it using the GitHub style"
}
```
