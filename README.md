# paper-list-for-M-LLMRec-VideoRec
a paper list about (M)LLM/Rec/VideoRec

每个论文以论文题目/录用会议/发布日期/summary/opinion/论文链接列出。

# For reference（GREEN）:
- LLMRec: Large Language Models with Graph Augmentation for Recommendation [[PDF](https://dl.acm.org/doi/pdf/10.1145/3616855.3635853)]  
  WSDM2024 Mar-24  
  使用openai的ada和davinci增强图数据，图片和文本编码器用的clip-vit和sentence-BERT  
  方向一致，问题是缺少视频模态而且api收费  
- Rec-GPT4V: Multimodal Recommendation with Large Vision-Language Models   [[PDF](https://arxiv.org/pdf/2402.08670.pdf)]  
  arxiv Feb-24  
  使用gpt和llava做推荐系统  
  强相关，使用了LLAVA，可以参考  
- Can Small Language Models be Good Reasoners for Sequential Recommendation [[PDF](https://arxiv.org/pdf/2403.04260.pdf)]  
  arxiv Mar-24  
  知识蒸馏训练LLaMA2-7B  
  框架可学，拿stepbystep做novelty不足  
- Towards Efficient and Effective Unlearning of Large Language Models for Recommendation [[PDF](https://arxiv.org/pdf/2403.03536v1.pdf)]  
  arxiv Mar-24  
  让LLM具备推荐能力后，忘记具体数据  
  少参数学习，多教师学习，可学  
- Visual instruction tuning [[PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/6dcf277ea32ce3288914faf369fe6de0-Paper-Conference.pdf)]  
  NeurIPS2023 Nov-23  
  LLAVA  
  开源多模态大模型   
- Multi-modal self-supervised learning for recommendation [[PDF](https://dl.acm.org/doi/pdf/10.1145/3543507.3583206)]  
  WWW2023 Apr-23  
  对抗性扰动，多模态对比学习，代码开源  
  可以看一下模型，编码器选择，效果  
- ONCE: Boosting Content-based Recommendation with Both Open- and Closed-source Large Language Models [[PDF](https://dl.acm.org/doi/pdf/10.1145/3616855.3635845)]  
  WSDM2024 Mar-24  
  探索开源闭源LLMRec，1张A100（80G）训练LLaVa所有参数  
  看一下pipeline，思考他们的novelty  
- Repeated Padding as Data Augmentation for Sequential Recommendation [[PDF](https://arxiv.org/pdf/2403.06372v1.pdf)]  
  arxiv Mar-24  
  把sequential rec的padding用重复序列填满，效果竟然有不小提升  
  特别有意思，感觉可以用，细细一想。。。他不就是把短序列重复然后变成了类似重复购买的数据吗。。。这不算数据造假吗？  
- NineRec: A Benchmark Dataset Suite for Evaluating Transferable Recommendation [[PDF](https://arxiv.org/pdf/2309.07705.pdf)]  
  TPAMI Mar-24  
  500k and 2M user规模的cove、标题数据集，来自于b站和其他平台  
  看了一下与发表版，其中附录表5有成本，可以关注一下完全版的成本部分以及PT的效果  
- Self-Attentive Sequential Recommendation [[PDF](https://arxiv.org/pdf/1808.09781.pdf)]  
  IEEE2018 Nov-18  
  将self-attention用到了rec的用户交互序列，拉近相同序列中embedding的关系  
  baseline，是否意味着初始的embedding是不重要的？最后embedding里面都是序列信息？  
- PromptMM: Multi-Modal Knowledge Distillation for Recommendation with Prompt-Tuning [[PDF](https://arxiv.org/pdf/2402.17188v1.pdf)]  
  WWW2024 Feb-24  
  使用知识蒸馏简化强化推荐系统  
  没有使用大语言模型的，但是是多模态推荐  

# expandable（YELLOW）  
- Mamba4Rec: Towards Efficient Sequential Recommendation with Selective State Space Models [[PDF](https://arxiv.org/pdf/2403.03900v1.pdf)]  
  arxiv Mar-24  
  使用mamba做推荐系统  
  待看  
- Mamba: Linear-time sequence modeling with selective state spaces [[PDF](https://arxiv.org/ftp/arxiv/papers/2312/2312.00752.pdf)]  
  Mamba模型  
  相关词是选择状态机和微分方程  

# not related/bad(RED)  
- Uncovering the Deep Filter Bubble: Narrow Exposure in Short-Video Recommendation [[PDF](https://arxiv.org/pdf/2403.04511.pdf)]  
  arxiv Mar-24  
  关于短视频推荐中的深度过滤泡问题的研究  
  感觉不相关  
- Towards Open-World Recommendation with Knowledge Augmentation from Large Language Models [[PDF](https://arxiv.org/pdf/2306.10933v4.pdf)]  
  arxiv Dec-23  
  直接用LLM去生成open的数据集，进行训练  
  创新不足      
- ReLLa: Retrieval-enhanced Large Language Models for Lifelong Sequential Behavior Comprehension in Recommendation [[PDF](https://arxiv.org/pdf/2308.11131.pdf)]  
  arxiv Aug-23  
  RAG，开源代码  
  no novelty  
- KELLMRec: Knowledge-Enhanced Large Language Models for Recommendation [[PDF](https://arxiv.org/pdf/2403.06642.pdf)]  
  arxiv Mar-24  
  LLM做rec的知识增强，对比学习框架  
  南京大学和微信的工作，做的事微信文章推荐的工作，可参考，但缺乏novelty，不开源·  
- CoRAL: Collaborative Retrieval-Augmented Large Language Models Improve  Long-tail Recommendation [[PDF](https://arxiv.org/pdf/2403.06447v1.pdf)]  
  arxiv Mar-24  
  未开源，强化学习框架，直接使用LLM做Recsys  
  方法论写的看不懂，直接用LLM做Rec一般效果不好  
- Pre-Trained Model Recommendation for Downstream Fine-tuning [[PDF](https://arxiv.org/pdf/2403.06382v1.pdf)]  
  arxiv Mar-24  
  提出了一个评价LLM的framework  
  不相关    
