# TiconvQA：Construction of high-quality Tibetan language dataset for conversational reading comprehension

TiconvQA（Tibetan Conversational Question Answering）是一个面向文本理解的藏文多轮对话数据集，其中包含了20,358个对话问答回合，涵盖地理、人物和新闻等三个不同领域的内容。每个对话回合都包括一个问题、一个答案以及相关的证据文本。

我们从三个不同领域的数据源中收集了段落，用于构建TiconvQA数据集：分别是来自云藏百科[https://baike.yongzin.com](https://baike.yongzin.com)的人物和地理词条信息，以及来自中国藏族网通[https://ti.tibet3.com](https://ti.tibet3.com)的新闻文章。


## 声明
为了进一步推动藏语对话式机器阅读理解的发展，并满足该领域相关研究人员的数据需求，我们选择将TiconvQA的一部分数据开放源代码。该开放数据集包含根据977个藏文段落构建的10,000个对话问答回合，其中包括根据地理领域的155个藏文段落构建2000个对话问答回合;根据人物领域的333个藏文段落构建包含3000个对话问答回合;根据新闻领域的489个藏文段落构建的5000个对话问答回合。
公开数据集仅供学习研究之用。如果您打算在商业场景中使用，请联系作者获得许可，并在得到作者同意后使用相关语料。

- TiconvQA.json：我们的数据集以 JSON 格式存储。每个故事包含一个唯一的标识符（id），故事的名称（storyname）以及故事内容（story）。问题和答案以对话形式组织，每个对话包含多个轮次（turn_id），每个轮次包含对话提出的问题或回答。答案中包含了正确的答案内容以及在故事中的起止位置（span_start 和 span_end）即证据部分，以及从故事中抽取出的相关文本片段（span_text）。

## 完整TiconvQA数据集构建规模如下：
| 主题   |文章段落数 | QA对数  |
|--------|------------|---------|
| 人物   | 669        | 5942    |
| 地理   | 441        | 4309    |
| 新闻   | 1010       | 10169   |
| TiconvQA-总| 2120       | 20358   |

## 联系方式
电子邮箱：tracy.yuan.sun@gmail.com
