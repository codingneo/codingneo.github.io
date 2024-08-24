## Text2SQL for Analytics with LLM

### Introduction
Due to a plugin called `jekyll-titles-from-headings` which is supported by GitHub Pages by default. The above header (in the markdown file) will be automatically used as the pages title.

If the file does not start with a header, then the post title will be derived from the filename.

This is a sample blog post. You can talk about all sorts of fun things here.

---

### Reference
#### Surveys
1. Zijin Hong, Zheng Yuan, Qinggang Zhang, Hao Chen, Junnan Dong, Feiran Huang, and Xiao Huang, Next-Generation Interfaces: A Survey of LLM-based Text-to-SQL, 2024-arXiv. [[paper](https://arxiv.org/html/2406.08426)]
2. Liang Shi, Zhengju Tang, Man Zhang, xiaotong Zhang and Zhi Yang, A Survey on Employing Large Language Models for Text-to-SQL Tasks, 2024-arXiv. [[paper](https://arxiv.org/pdf/2407.15186)]
3. Weixu Zhang, Yifei Wang, Yuanfeng Song, Victor Junqiu Wei, Yuxing Tian, Yiyan Qi, Jonathan H. Chan, Raymond Chi-Wing Wong and Haiqin Yang, Natural Language Interfaces for Tabular Data Querying and Visualization: A Survey, 2023-arXiv. [[paper](https://arxiv.org/abs/2310.17894)]

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
