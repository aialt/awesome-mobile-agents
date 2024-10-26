
# Recent Trends in Multimodal Mobile Agents: A Survey

![Example Image](img.webp)



## Datasets and Benchmarks

| Dataset                      | Templates | Attach | Task             | Reward         | Platform          |
|------------------------------|------------|--------|------------------|----------------|-------------------|
| **Static Dataset**           |            |        |                  |                |                   |
| RICOSCA (Deka et al., 2017)  | 259k       | -      | Grounding        | -              | Android           |
| ANDROIDHOWTO (Deka et al., 2017) | 10k    | -      | Extraction       | -              | Android           |
| PixelHelp (Li et al., 2020a) | 187        | -      | Apps             | -              | Android           |
| Screen2Words (Wang et al., 2021) | 112k   | XML    | Summarization    | -              | Android           |
| META-GUI (Lee et al., 2021)  | 1,125      | -      | Apps+Web         | -              | Android           |
| MoTIF (Wang et al., 2022)    | 4,707      | -      | Apps             | -              | Android           |
| UGIF (Venkatesh et al., 2022) | 4184     | XML    | Grounding        | -              | Android           |
| AitW (Rawles et al., 2024b)  | 30k        | -      | Apps+Web         | -              | Android           |
| AitZ (Zhang et al., 2024b)   | 2504       | -      | Apps+Web         | -              | Android           |
| AMEX (Chai et al., 2024)     | 3k         | XML    | Apps+Web         | -              | Android           |
| Ferret-UI (You et al., 2024) | 120k       | -      | Apps             | -              | IOS               |
| GUI-World (Chen et al., 2024a) | 12k      | -      | Apps+Web         | -              | Multi Platforms   |
| Mobile3M (Chen et al., 2024a) | 3M        | -      | Apps             | -              | Android           |
| Odyssey (Lu et al., 2024)    | 7735       | -      | Apps+Web         | -              | Multi Platforms   |
| **Interactive Environment**  |            |        |                  |                |                   |
| MiniWoB++ (Liu et al., 2018) | 114        | -      | Web (synthetic)  | Sparse Rewards | -                 |
| AndroidEnv (Toyama et al., 2021) | 100    | -      | Apps             | Sparse Rewards | Android           |
| AppBuddy (Shvo et al., 2021) | 35         | -      | Apps             | Sparse Rewards | Android           |
| Mobile-Env (Zhang et al., 2023a) | 224    | XML    | Apps+Web         | Dense Rewards  | Android           |
| AndroidArena (Wang et al., 2024c) | 221   | XML    | Apps+Web         | Sparse Rewards | Android           |
| AndroidWorld (Rawles et al., 2024a) | 116 | -      | Apps+Web         | Sparse Rewards | Android           |
| DroidTask (Wen et al., 2024) | 158        | XML    | Apps+Web         | -              | Android           |
| B-MoCA (Lee et al., 2024)    | 60         | XML    | Apps+Web         | -              | Android           |
| Mobile-Bench (Deng et al., 2024a) | 832   | XML    | Apps+Web         | -              | Android           |

*Comparison of various platforms based on templates, attach information, tasks, rewards, and supported platforms. In particular, the reward mechanisms are categorized as Sparse Rewards and Dense Rewards. Sparse Rewards are given only when the agent reaches a specific goal or completes the task, making learning more difficult due to the lack of immediate feedback. On the other hand, Dense Rewards provides feedback after each step or action, helping the agent learn the correct strategy more quickly.*

For general OS systems, see the section on [`General OS Systems`](#general-os-systems).

## Mobile Agents

| Method                        | Input Type  | Model     | Training   | Memory | Multi-agents |
|-------------------------------|-------------|-----------|------------|--------|--------------|
| **Prompt-based Methods**      |             |           |            |        |              |
| ResponsibleTA (Zhang et al., 2023c) | Image&Text | GPT-4     | None       | ✓      | ✗            |
| DroidGPT (Wen et al., 2023b)  | Text        | ChatGPT   | None       | ✗      | ✗            |
| AppAgent (Yang et al., 2023)  | Image&Text  | GPT-4     | None       | ✓      | ✗            |
| MobileAgent (Wang et al., 2024b) | Image&Text | GPT-4   | None       | ✓      | ✗            |
| MobileAgent v2 (Wang et al., 2024a) | Image&Text | GPT-4 | None  | ✓      | ✓            |
| AutoDroid (Wen et al., 2024)  | Image&Text  | GPT-4     | None       | ✓      | ✗            |
| AppAgent V2 (Li et al., 2024) | Image&Text  | GPT-4     | None       | ✓      | ✗            |
| VLUI (Lee et al., 2024)       | Image&Text  | GPT4      | None       | ✗      | ✗            |
| **Training-based Methods**    |             |           |            |        |              |
| MiniWob (Liu et al., 2018)    | Image       | DOMNET    | RL-based   | ✗      | ✗            |
| MetaGUI (Sun et al., 2022)    | Image&Text  | VLM       | Pre-trained| ✗      | ✗            |
| CogAgent (Hong et al., 2023)  | Image&Text  | CogVLM    | Pre-trained| ✗      | ✗            |
| AutoGUI (Zhang and Zhang, 2023) | Image&Text | MMT5     | Finetune   | ✓      | ✗            |
| ResponsibleTA (Zhang et al., 2023c) | Image&Text | VLM   | Finetune   | ✓      | ✗            |
| UI-VLM (Dorka et al., 2024)   | Image&Text  | LLaMA     | Finetune   | ✓      | ✗            |
| Coco-Agent (Ma et al., 2024)  | Image&Text  | MMT5      | Finetune   | ✓      | ✗            |
| DigiRL (Bai et al., 2024)     | Image&Text  | MMT5      | RL-based   | ✗      | ✗            |
| SphAgent (Chai et al., 2024)  | Image&Text  | VLM       | Finetune   | ✗      | ✗            |
| Octopus v2 (Chen and Li, 2024) | Text       | Gemma     | Finetune   | ✗      | ✗            |
| Octo-planner (Chen et al., 2024c) | Text    | Gemma     | Finetune   | ✗      | ✓            |
| MobileVLM (Wu et al., 2024)   | Image&Text  | Qwen-VL   | Finetune   | ✓      | ✗            |
| OdysseyAgent (Lu et al., 2024) | Image&Text | Qwen-VL   | Finetune   | ✓      | ✗            |

*Comparison of Mobile Agents: A Detailed Overview of Input Types, Models, Training Methods, Memory Capabilities, and Multi-agent Support.*




% Unimodal MOBILE AGENTS
% Multimodal MOBILE AGENTS 

## Base Model

- CogVLM: Visual Expert for Pretrained Language Models https://arxiv.org/abs/2311.03079
- MiniCPM: Unveiling the Potential of Small Language Models with Scalable Training Strategies https://arxiv.org/abs/2404.06395
- LLaVA-NeXT: Improved reasoning, OCR, and world knowledge https://llava-vl.github.io/blog/2024-01-30-llava-next/
- LLaVA-OneVision: Easy Visual Task Transfer https://arxiv.org/abs/2408.03326
- SeeClick: Harnessing GUI Grounding for Advanced Visual GUI Agents (ACL2024) https://arxiv.org/abs/2401.10935
- CogAgent: A Visual Language Model for GUI Agents http://arxiv.org/abs/2312.08914



## Prompt Based Framework

- AppAgent: Multimodal Agents as Smartphone Users https://arxiv.org/abs/2312.13771
- Mobile-Agent: Autonomous Multi-Modal Mobile Device Agent with Visual Perception https://arxiv.org/abs/2401.16158
- UFO: A UI-Focused Agent for Windows OS Interaction https://arxiv.org/abs/2402.07939
- OS-Copilot: Towards Generalist Computer Agents with Self-Improvement https://arxiv.org/abs/2402.07456
- MMAC-Copilot: Multi-modal Agent Collaboration Operating System Copilot https://arxiv.org/abs/2404.18074
- A Real-World WebAgent with Planning, Long Context Understanding, and Program Synthesis http://arxiv.org/abs/2307.12856
- OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web http://arxiv.org/abs/2402.17553
- Comprehensive Cognitive LLM Agent for Smartphone GUI Automation http://arxiv.org/abs/2402.11941
- Tree Search for Language Model Agents https://arxiv.org/abs/2407.01476



## LLM-SFT Based Framework
- CogAgent: A Visual Language Model for GUI Agents https://arxiv.org/abs/2312.08914
- ScreenAI: A Vision-Language Model for UI and Infographics Understanding https://arxiv.org/abs/2402.04615
- TRAINING A VISION LANGUAGE MODEL AS SMARTPHONE ASSISTANT (ICLR 2024) https://arxiv.org/abs/2404.08755
- AGENTOHANA: Designing a Unified Data and Training Pipeline for Effective Agent Learning https://arxiv.org/abs/2402.15506

- Towards General Computer Control: A Multimodal Agent for Red Dead Redemption II as a Case Study https://arxiv.org/abs/2403.03186
- Scaling Instructable Agents Across Many Simulated Worlds [link to technical report](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/sima-generalist-ai-agent-for-3d-virtual-environments/Scaling%20Instructable%20Agents%20Across%20Many%20Simulated%20Worlds.pdf)
- Octo-planner: On-device Language Model for Planner-Action Agents https://arxiv.org/abs/2406.18082
- Octopus v2: On-device language model for super agent https://arxiv.org/pdf/2404.01744.pdf
- You Only Look at Screens: Multimodal Chain-of-Action Agents https://arxiv.org/abs/2309.11436 https://github.com/cooelf/Auto-GUI
- Comprehensive Cognitive LLM Agent for Smartphone GUI Automation http://arxiv.org/abs/2402.11941
- Improving Language Understanding from Screenshots http://arxiv.org/abs/2402.14073




## LLM-RL Based Framework

- Fine-Tuning Large Vision-Language Models as Decision-Making Agents via Reinforcement Learning https://arxiv.org/pdf/2405.10292
- DigiRL: Training In-The-Wild Device-Control Agents with Autonomous Reinforcement (NIPS2024) https://arxiv.org/abs/2406.11896





## UI understanding and Automation


- UIED: a hybrid tool for GUI element detection https://sidongfeng.github.io/papers/uied.pdf
- Object Detection for Graphical User Interface: Old Fashioned or Deep Learning or a Combination? https://arxiv.org/abs/2008.05132
- AutoDroid: LLM-powered Task Automation in Android  CHI 2024 https://arxiv.org/abs/2308.15272
- Spotlight: Mobile UI Understanding using Vision-Language Models with a Focus    ICLR 2023 https://arxiv.org/abs/2209.14927
- VUT: Versatile UI Transformer for Multimodal Multi-Task User Interface Modeling    ICLR 2022 https://arxiv.org/abs/2112.05692
- Widget Captioning: Generating Natural Language Description for Mobile User Interface Elements    EMNLP 2020 https://arxiv.org/abs/2010.04295
- Screen Recognition: Creating Accessibility Metadata for Mobile Applications from Pixels       CHI 2021 https://arxiv.org/abs/2101.04893
- Enabling Conversational Interaction with Mobile UI Using Large Language Models     CHI 2023 https://arxiv.org/abs/2209.08655
- Screen2Words: Automatic Mobile UI Summarization with Multimodal Learning    UIST 2021 https://arxiv.org/abs/2108.03353
- Kite: Building Conversational Bots from Mobile Apps    Mobisys 2018 https://dl.acm.org/doi/10.1145/3210240.3210339
- META-GUI: Towards Multi-modal Conversational Agents on Mobile GUI https://arxiv.org/abs/2205.11029
- DroidBot-GPT: GPT-powered UI Automation for Android https://arxiv.org/abs/2304.07061
- Responsible Task Automation: Empowering Large Language Models as Responsible Task Automation https://arxiv.org/abs/2306.01242
- Personal LLM Agents: Insights and Survey about the Capability, Efficiency and Security https://arxiv.org/abs/2401.05459
- MMAC-Copilot: Multi-modal Agent Collaboration Operating System Copilot https://chatpaper.com/chatpaper/zh-CN/paper/17441
- Screen2Words: Automatic Mobile UI Summarization with Multimodal Learning http://arxiv.org/abs/2108.03353





## Dataset and Benchmark

### 2017
- Scaling Instructable Agents Across Many Simulated Worlds (2017) https://arxiv.org/abs/2404.10179

### 2022
- MiniWoB++ / Success Rate (2022) https://miniwob.farama.org/ https://arxiv.org/abs/1802.08802

### 2023
- MoTIF: A Dataset for Interactive Vision-Language Navigation with Unknown Command Feasibility (2023) https://arxiv.org/abs/2202.02312
- IND2WEB: Towards a Generalist Agent for the Web (2023) https://arxiv.org/abs/2306.06070
- WebArena: A Realistic Web Environment for Building Autonomous Agents (2023) https://arxiv.org/abs/2307.13854


 
### 2024
- Android in the Wild: A Large-Scale Dataset for Android Device Control (2024) https://arxiv.org/abs/2307.10088
- AndroidWorld: A Dynamic Benchmarking Environment for Autonomous Agents / Success Rate https://google-research.github.io/android_world/
- OSWORLD: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments / Success Rate https://arxiv.org/abs/2404.07972
- ScreenAgent: A Vision Language Model-driven Computer Control Agent (ACL2024) https://arxiv.org/abs/2402.07945
- OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web / Sequence score https://arxiv.org/abs/2402.17553
- Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs https://arxiv.org/abs/2404.05719
- AutoUI: You Only Look at Screens: Multimodal Chain-of-Action Agents (ACL2024) https://arxiv.org/abs/2309.11436
- GUI-WORLD: A Dataset for GUI-oriented Multimodal LLM-based Agents https://arxiv.org/abs/2406.10819


- AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents (ACL2024) https://arxiv.org/abs/2407.18901
- Mobile-Bench: An Evaluation Benchmark for LLM-based Mobile Agents (ACL2024) https://arxiv.org/abs/2407.00993
- VisualWebArena: Evaluating Multimodal Agents on Realistic Visually Grounded Web Tasks (ACL2024) https://arxiv.org/abs/2401.13649
- WebCanvas: Benchmarking Web Agents in Online Environments https://arxiv.org/abs/2406.12373
- MobileAgentBench: An Efficient and User-Friendly Benchmark for Mobile LLM Agents https://arxiv.org/abs/2406.08184
- GUICourse: From General Vision Language Model to Versatile GUI Agent https://arxiv.org/abs/2406.11317
 

- Android in the Zoo: Chain-of-Action-Thought for GUI Agents http://arxiv.org/abs/2403.02713
- AndroidEnv: A Reinforcement Learning Platform for Android http://arxiv.org/abs/2105.13231 
- AgentStudio: A Toolkit for Building General Virtual Agents https://arxiv.org/abs/2403.17918
- VisualWebBench: How Far Have Multimodal LLMs Evolved in Web Page Understanding and Grounding? https://arxiv.org/abs/2404.05955
- OS-Copilot: Towards Generalist Computer Agents with Self-Improvement https://arxiv.org/abs/2402.07456
- E-ANT: A Large-Scale Dataset for Efficient Automatic GUI NavigaTion https://arxiv.org/pdf/2406.14250
- AndroidWorld https://github.com/google-research/android_world
- AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents https://arxiv.org/abs/2407.18901 https://appworld.dev/
- VisualWebBench: How Far Have Multimodal LLMs Evolved in Web Page Understanding and Grounding? https://arxiv.org/abs/2404.05955
- Mobile-Env: An Evaluation Platform and Benchmark for LLM-GUI Interaction https://arxiv.org/abs/2305.08144
- OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments https://arxiv.org/abs/2404.07972
- Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs https://arxiv.org/abs/2404.05719


## To-Do List



- LaVague: Web Agent framework for builders https://github.com/lavague-ai/LaVague
- WebLlama: https://github.com/McGill-NLP/webllama
- AutoCrawler: A Progressive Understanding Web Agent for Web Crawler Generation https://arxiv.org/abs/2404.12753

- WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models (ACL2024) https://arxiv.org/abs/2401.13919
- Tuning Large Multimodal Models for Videos using Reinforcement Learning from AI Feedback (ACL2024) https://arxiv.org/abs/2402.03746




- ReALM: Reference Resolution As Language Modeling https://arxiv.org/abs/2403.20329
- AutoWebGLM: Bootstrap And Reinforce A Large Language Model-based Web Navigating Agent https://arxiv.org/abs/2404.03648




- AutoDroid: LLM-powered Task Automation in Android https://arxiv.org/abs/2308.15272
- Fine-Tuning Large Vision-Language Models as Decision-Making Agents via Reinforcement Learning https://rl4vlm.github.io
- WebArena: A Realistic Web Environment for Building Autonomous Agents https://arxiv.org/abs/2307.13854
- Synapse: Trajectory-as-Exemplar Prompting with Memory for Computer Control https://openreview.net/pdf?id=Pc8AU1aF5e
- gpt-computer-assistant https://github.com/onuratakan/gpt-computer-assistant

- GUI Odyssey: A Comprehensive Dataset for Cross-App GUI Navigation on Mobile Devices https://github.com/OpenGVLab/GUI-Odyssey
- ASSISTGUI: Task-Oriented PC Graphical User Interface Automation https://showlab.github.io/assistgui/

- Read Anywhere Pointed: Layout-aware GUI Screen Reading with Tree-of-Lens Grounding https://arxiv.org/abs/2406.19263
- Cradle: Empowering Foundation Agents Towards General Computer Control https://arxiv.org/abs/2403.03186



# Citation

```bib
@article{wu2024curriculum,
  title={Curriculum Learning with Quality-Driven Data Selection},
  author={Wu, Biao and Meng, Fang and Chen, Ling},
  journal={arXiv preprint arXiv:2407.00102},
  year={2024}
}
```


--- 

## Appendix

### General OS Systems

 | Dataset                      | Templates | Attach | Task             | Reward         | Platform          |
|------------------------------|------------|--------|------------------|----------------|-------------------|
| **Static Dataset**           |            |        |                  |                |                   |
| RICOSCA (Deka et al., 2017)  | 259k       | -      | Grounding        | -              | Android           |
| ANDROIDHOWTO (Deka et al., 2017) | 10k    | -      | Extraction       | -              | Android           |
| PixelHelp (Li et al., 2020a) | 187        | -      | Apps             | -              | Android           |
| WebSRC (Chen et al., 2021)   | 400k       | HTML   | Web              | -              | Windows           |
| Screen2words (Wang et al., 2021) | 112k  | XML    | Summarization    | -              | Android           |
| META-GUI (Lee et al., 2021)  | 1,125      | -      | Apps+Web         | -              | Android           |
| MoTIF (Wang et al., 2022)    | 4,707      | -      | Apps             | -              | Android           |
| UGIF (Venkatesh et al., 2022) | 4184     | XML    | Grounding        | -              | Android           |
| WebUI (Wu et al., 2023)      | 400k       | HTML   | Web              | -              | Windows           |
| Mind2Web (Deng et al., 2024) | 2,350      | HTML   | Web              | -              | Windows           |
| AitW (Rawles et al., 2024b)  | 30k        | -      | Apps+Web         | -              | Android           |
| AitZ (Zhang et al., 2024b)   | 2504       | -      | Apps+Web         | -              | Android           |
| AMEX (Chai et al., 2024)     | 3k         | XML    | Apps+Web         | -              | Android           |
| Ferret-UI (You et al., 2024) | 120k       | HTML   | Apps             | -              | Multi-Platforms   |
| OmniAct (Kapoor et al., 2024) | 9802      | Org/Seg | Web             | -              | Windows           |
| WebLINX (Roßner et al., 2020) | 2,337     | HTML   | Web              | -              | Windows           |
| ScreenAgent (Niu et al., 2024) | 3005     | HTML   | Web              | -              | Windows           |
| GUI-World (Chen et al., 2024a) | 12k      | -      | Apps+Web         | -              | Multi Platforms   |
| Mobile3M (Chen et al., 2024a) | 3M        | -      | Apps             | -              | Android           |
| **Interactive Environment**  |            |        |                  |                |                   |
| MiniWoB++ (Liu et al., 2018) | 114        | -      | Web (synthetic)  | HTML/JS state  | -                 |
| AndroidEnv (Toyama et al., 2021) | 100    | -      | Apps             | Device state   | Android           |
| WebShop (Yao et al., 2022a)  | 12k        | -      | Web              | Product Attrs Match | Windows     |
| WebArena (Zhou et al., 2023) | 241        | HTML   | Web              | url/text-match | Windows           |
| Mobile-Env (Zhang et al., 2023a) | 224    | XML    | Apps+Web         | Intermediate state | Android      |
| VisualWebArena (Koh et al., 2024) | 314   | HTML   | Web              | url/text/image-match | Windows     |
| Ferret-UI (You et al., 2024) | 314        | HTML   | Web              | url/text/image-match | Windows     |
| AndroidArena (Wang et al., 2024c) | 221   | XML    | Apps+Web         | Device state   | Android           |
| AndroidWorld (Rawles et al., 2024a) | 116 | -      | Apps+Web         | Device state   | Android           |
| OSWorld (Xie et al., 2024)   | 369        | -      | Web              | Device/Cloud state | Linux         |
| DroidTask (Wen et al., 2024) | 158        | XML    | Apps+Web         | -              | Android           |

*Comparison of various platforms based on parallelization, templates, tasks per template, rewards, and supported OS.*
