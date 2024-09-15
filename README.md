# CriticalThinking-Finetuning-Dataset
## Introduction：
This dataset is designed for fine-tuning large language models to enhance users' critical thinking and reasoning skills. It includes structured Q&A sessions, role-playing scenarios, and debates that challenge users to analyze, evaluate, and construct reasoned arguments. The dataset promotes in-depth thinking and encourages reflective learning, making it ideal for applications in education, tutoring, and skill development.
本数据集旨在通过微调大语言模型来提升用户的批判性思维和推理能力。数据集包括结构化的问答环节、角色扮演场景和辩论，旨在引导用户进行分析、评估和构建有逻辑的论证。该数据集鼓励深度思考和反思性学习，特别适用于教育、辅导以及技能开发等领域的应用

## Dataset Contents
The dataset consists of various dialogue examples intended to stimulate critical thinking. It includes the following types of interactions:
该数据集由各种对话示例组成，旨在激发批判性思维。它包括以下类型的交互：
- Q&A Sessions: Structured question and answer formats that guide the user in logical thinking and encourage deeper exploration of topics.
- Role-Playing Scenarios: Users are assigned different roles in hypothetical situations, encouraging them to evaluate problems from multiple perspectives.
- Debates: The dataset contains debate structures where users argue for or against a given proposition, sharpening their reasoning skills.

## Example Structure:
### Q&A Session:
```json
      {
        "role": "user",
        "content": "抽象艺术如何挑战了传统的艺术观念？"
      },
      {
        "role": "assistant",
        "content": "很好的问题！首先你能告诉我创新活动在日常生活中的一些例子吗？"
      },
      {
        "role": "user",
        "content": "比如吸尘器的发明，使得大家不再需要手动扫地。"
      },
      {
        "role": "assistant",
        "content": "非常好，就像吸尘器的发明改变了我们的生活方式一样，抽象艺术也改变了艺术的发展。抽象艺术与传统艺术有何不同，你觉得呢？"
      }
```

### Playing Scenario: 
```json
            [   "请和我开始批判性思维情景对话训练",
                "今天我们来进行一个批判性思维训练。想象一下，你身处一个城市规划委员会的会议中，讨论关于城市公共交通改革的提案。在场有几位虚拟角色：市长（主张全面引入无人驾驶公交）、环保倡导者李华（强调减少碳排放）、公交司机张师傅（担忧失业问题）、以及普通市民小红（关心出行便利性）。请选择一位角色扮演。"
            ],
            [
                "我想扮演环保倡导者李华。",
                "很好，李华。现在，有一个观点是“无人驾驶公交能显著提高效率并减少交通拥堵”，你怎么看？"
            ],
            [
                "作为李华，我完全同意这个观点。无人驾驶公交能按照最优化路线行驶，减少人为错误导致的延误，同时因为智能化调度，能更高效地分配车辆，缓解拥堵，进而减少汽车排放，符合我的环保主张。",
                "很好的分析，李华。接下来，我们深入一点。我注意到你在谈论中提到了“最优化路线”和“减少排放”。请具体解释一下这两个限定词对你立场的重要性。"
            ]
```

### Debate Example:
```json
 [              "请和我开始一轮辩论。",
                "今天我们来进行一场辩论。辩题是：“网络课程应该成为主流教育形式。”正方认为网络课程提供了灵活性和可访问性，是未来教育的趋势。反方则认为网络课程无法提供足够的互动和实践机会，不应成为主流教育形式。你想支持哪一方？"
            ],
            [
                "我支持正方。",
                "很好，请开始你的第一轮发言。"
            ],
            [
                "网络课程提供了很大的灵活性。学生可以根据自己的时间表自由安排学习，而且可以接触到世界各地最好的教育资源。",
                "灵活性确实是网络课程的优点之一。然而，网络学习的过度灵活性可能会导致学生缺乏自律，这不是一个问题吗？学生可能因为缺乏固定的学习结构而学习不足。"
            ]
```

## Usage

## File Structure
The repository is organized as follows:

```bash

Critical-Thinking-Training-Dataset/
│
├── data/
│   ├── qa_sessions.json        # Contains the structured Q&A sessions
│   ├── role_play.json          # Contains role-playing scenario data
│   ├── debates.json            # Contains debate data for critical thinking exercises
│
├── README.md                   # Overview and instructions
├── LICENSE                     # Licensing information
└── requirements.txt            # Any dependencies required for using the dataset
```

## Contribution
We welcome contributions from the community. If you would like to improve this dataset or have suggestions, feel free to submit a pull request or open an issue.
我们欢迎社区的贡献。如果您想改进此数据集或有任何建议，请随时提交拉取请求或打开问题。

## License
This dataset is released under the MIT License. You are free to use, modify, and distribute it for any purpose, as long as you provide attribution to the original authors.
此数据集在 MIT 许可证下发布。您可以出于任何目的自由使用、修改和分发它，只要您提供原作者的署名即可。
