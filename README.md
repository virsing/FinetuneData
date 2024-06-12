# FinetuneData
general sft data

# 通用预训练数据
1、FineWeb、[blog]（https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1）（预训练）
Hugging Face的一个团队发布了FineWeb数据集（15万亿 tokens，44TB）。技术报告详细介绍了该数据集的加工决策过程：FineWeb源自96个CommonCrawl快照，如何通过缜密的去重和过滤策略，比其他开放预训练数据集产生了表现更好的LLM的。

2、[huggingface/cosmopedia](https://huggingface.co/datasets/HuggingFaceTB/cosmopedia)、[github](https://github.com/huggingface/cosmopedia)、[blog](https://huggingface.co/blog/cosmopedia)  （预训练）
Cosmopedia是一个由Mixtral-8x7B-Instruct-v0.1生成的合成textbooks、博客文章、故事、帖子和WikiHow文章的预训练数据集。该数据集包含超过3000万个文件和250亿个tokens（92.2 GB），使其成为迄今为止最大的开放合成数据集。


# 通用sft data
1、[teknium/OpenHermes-2.5](https://huggingface.co/datasets/teknium/OpenHermes-2.5)  
Open Hermes 2/2.5 模型在 SOTA LLM 的基础上取得了重大进步，并以许多开源数据集和自定义创建的合成数据集的精确编译和管理为基础。一共100w条数据（1.94G）。
Dataset Sources

- Airoboros 2.2 | By Jon Durbin [airoboros](https://huggingface.co/datasets/jondurbin/airoboros-2.2)
- CamelAI Domain Expert Datasets (Physics, Math, Chemistry & Biology) | By [CamelAI](https://huggingface.co/camel-ai)
- ChatBot Arena (GPT-4 Only) | By LMSys: [lmsys-chat-1m](https://huggingface.co/datasets/lmsys/lmsys-chat-1m)
- Collective Cognition (09-11-2023) | By Teknium: [CollectiveCognition](https://huggingface.co/datasets/CollectiveCognition/chats-data-2023-09-22)
- CoT Alpaca GPT4 | I have lost the source page for this dataset, sorry
- Evol Instruct 70K && 140K |By WizardLM: [70K](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_70k) [140k](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_V2_196k)
- Glaive Code Assistant | By Sahil & Glaive: [glaive-code-assistant](https://huggingface.co/datasets/glaiveai/glaive-code-assistant)
- GPT4-LLM | By Baolin Peng*, Chunyuan Li*, Pengcheng He*, Michel Galley, Jianfeng Gao [GPT4-LLM-Cleaned](https://huggingface.co/datasets/teknium/GPT4-LLM-Cleaned)
- GPTeacher | By Teknium & Kuruminha: [GPTeacher](https://github.com/teknium1/GPTeacher)
- Medical Tasks | By CogStack: [OpenGPT](https://github.com/CogStack/OpenGPT)
- MetaMath 40k | By MetaMath: [MetaMathQA](https://huggingface.co/datasets/meta-math/MetaMathQA)
- SlimOrca 550K | By Wing Lian and Guan Wang and Bleys Goodson and Eugene Pentland and Austin Cook and Chanvichet Vong and Teknium: [SlimOrca](https://huggingface.co/datasets/Open-Orca/SlimOrca)
- Platypus | By Garage-bAInd: [Open-Platypus](https://huggingface.co/datasets/garage-bAInd/Open-Platypus)
- ShareGPT (GPT4-Only) | By LMSys: [ShareGPT_Vicuna_unfiltered](https://huggingface.co/datasets/anon8231489123/ShareGPT_Vicuna_unfiltered)
- Unnatural Instructions GPT4

2、[TIGER-Lab/WebInstructSub](https://huggingface.co/datasets/TIGER-Lab/WebInstructSub)、[github](https://tiger-ai-lab.github.io/MAmmoTH2/)、[paper](https://tiger-ai-lab.github.io/MAmmoTH2/)  
微调数据集。网络语料库中存在大量高质量的教学数据，涵盖数学和科学等各个领域。三步流程包括从 Common Crawl 中调用文档、提取 QA 对并对其进行质量改进。这种方法产生了 1000 万个指令-响应对，为现有数据集提供了可扩展的替代方案，将精选的数据集命名为 WebInstruct。

3、MAmmoTH2、[项目地址]（https://tiger-ai-lab.github.io/MAmmoTH2/）、[paper](https://arxiv.org/abs/2405.03548)、[github](https://github.com/TIGER-AI-Lab/MAmmoTH2)  
作者提出了一种方法，从预训练网络语料库中高效地收集1000万条自然存在的指令数据，以增强大语言模型（LLM）的推理能力。作者的方法包括（1）检索相关文档，（2）提取指令-响应对，（3）使用开源LLM对提取的对进行精化。在这个数据集上对基础LLM进行微调，作者构建了MAmmoTH2模型，显著提升了推理基准测试的性能。特别是，MAmmoTH2-7B（Mistral）在MATH上的性能从11%提升至34%，在GSM8K上从36%提升至67%，而无需使用任何领域内数据进行训练。进一步在公共指令微调数据集上训练MAmmoTH2，得到了MAmmoTH2-Plus，实现了几个推理和聊天机器人基准测试的最新性能。作者的工作展示了如何在没有昂贵的人工注释或GPT-4精馏的情况下收集大规模、高质量的指令数据，为构建更好的指令微调数据提供了一个新范式。

