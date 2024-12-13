# Awesome Unified Multimodal Understanding and Generation
![12](https://github.com/user-attachments/assets/d12e541f-514d-481d-8d7f-91e793680fb6)

<img src="https://github.com/user-attachments/assets/d12e541f-514d-481d-8d7f-91e793680fb6" alt="Logo" style="width: 50%; max-width: 500px;"/>

<div align="center">
  <img src="https://github.com/user-attachments/assets/d12e541f-514d-481d-8d7f-91e793680fb6" alt="Logo" width="500"/>
</div>

A **curated list of papers, models, and resources** dedicated to **unified multimodal understanding and generation**, with a focus on research that seamlessly integrates multimodal comprehension (e.g., interpreting and aligning text, images, and other modalities) with the ability to generate high-quality multimodal outputs. This repository serves as a **comprehensive entry point** for researchers, engineers, and practitioners interested in developing models and systems that unify understanding and generation tasks across modalities.

By aggregating foundational concepts, cutting-edge frameworks, and state-of-the-art approaches—ranging from autoregressive modeling to diffusion-based techniques—this list encourages a holistic view of the field, fosters comparative studies, and supports the development of next-generation multimodal systems.

---

## Table of Contents

- [What is Unified Multimodal Understanding and Generation?](#what-is-unified-multimodal-understanding-and-generation)
- [Categories](#categories)
- [Previous Works on Multimodal Understanding and Generation](#previous-works-on-multimodal-understanding-and-generation)
  - [Multimodal Understanding](#multimodal-understanding)
  - [Multimodal Generation](#multimodal-generation)
    - [Auto-regressive Models](#auto-regressive-models)
    - [Diffusion Models](#diffusion-models)
- [Unified Multimodal Understanding and Generation](#unified-multimodal-understanding-and-generation)
- [Contributions](#contributions)
- [License](#license)

---

## What is Unified Multimodal Understanding and Generation?

**Unified multimodal understanding and generation** refers to modeling paradigms capable of both:

1. **Holistic Understanding**: Interpreting and aligning diverse modalities (e.g., text, images, audio, video) to extract semantic and contextual information.
   
2. **Coherent Generation**: Producing high-fidelity outputs in various modalities—such as generating images from textual descriptions, narrating a scene described visually, or handling complex multimodal dialogues.

A unified approach typically employs a single integrated model or tightly coupled framework to perform both understanding and generation. This can improve training efficiency, simplify pipelines, and potentially enhance performance across downstream tasks. Unified multimodal models are increasingly leveraging:

- **Autoregressive paradigms** (e.g., transformer-based models) for token-by-token prediction.
- **Diffusion-based methods** to iteratively refine samples, bridging the gap between understanding and generation processes.
- **Unified tokenization schemes** that represent different modalities within a common embedding space, enabling more natural cross-modal learning.

---

## Categories

1. **Multimodal Understanding**  
   Models and frameworks focusing on interpreting multimodal data, learning semantic alignments between text and images, performing visual reasoning, and extracting contextual information across modalities.

2. **Multimodal Generation**  
   Approaches centered on creating multimodal content, such as generating image captions, synthesizing images from textual prompts, or constructing multimodal narratives. Within this category, the landscape spans:
   - **Auto-regressive Models**: Sequential generation of tokens (pixels, words, etc.) conditioned on multimodal inputs.
   - **Diffusion Models**: Progressive noise-to-sample refinement, now adapted for multimodal tasks.

3. **Unified Frameworks**  
   Methods that combine both multimodal understanding and generation into a single coherent system. These frameworks often rely on innovative architectures, shared representations, or integrated training objectives to jointly handle comprehension and creation tasks.

---

## Previous Works on Multimodal Understanding and Generation

### Multimodal Understanding

- **[LLaVA](https://arxiv.org/abs/2305.06500)**: A large multimodal model that aligns vision and language for tasks like image captioning and VQA.
- **[MiniGPT-4](https://github.com/Vision-CAIR/MiniGPT-4)**: A lightweight vision-language model building upon GPT-4 capabilities to enable advanced multimodal reasoning and understanding.
- **[BLIP](https://arxiv.org/abs/2201.12086)**: Bootstrapping Language-Image Pre-training for unified understanding and grounded text generation.
- **[Deepseek-VL]**: Enhanced vision-language integration for improved cross-modal retrieval and question answering.
- **[InternVL](https://arxiv.org/abs/2301.03729)**: A scalable vision-language foundation model tailored for generalizable, interpretable multimodal tasks.
- **[Qwen-VL](https://arxiv.org/abs/2308.13084)**: A vision-language model improving semantic alignment and robust multimodal reasoning.

### Multimodal Generation

#### Auto-regressive Models

- **[PixelRNN / PixelCNN](https://arxiv.org/abs/1601.06759)**: Early pixel-level autoregressive models for image generation, foundational for subsequent multimodal extensions.
- **LLamagen**: A generative text model extended into multimodal settings, enabling conditional image and text generation.

#### Diffusion Models

##### Continuous Diffusion

- **[DDPM](https://arxiv.org/abs/2006.11239)**: Denoising Diffusion Probabilistic Models, a cornerstone in image generation, recently adapted for multimodal tasks.

##### Discrete Diffusion

- **[D3PM](https://arxiv.org/abs/2107.03006)**: Discrete diffusion models operating directly on discrete tokens, supporting token-based multimodal generation.
- **[MaskGIT](https://arxiv.org/abs/2202.04200)**: A mask-based generative model for filling in masked tokens, instrumental for unified multimodal pipelines.

---

## Unified Multimodal Understanding and Generation

Below are recent works that integrate multimodal understanding and generation in a single framework, often combining autoregressive modeling, diffusion principles, and unified tokenization to achieve end-to-end performance:

- **[DreamLLM (2023)](https://arxiv.org/abs/2309.11499)**  
  *Runpei Dong et al.*  
  **Key Insight**: Moves beyond pipeline-based integrations by proposing a synergistic approach that simultaneously handles multimodal comprehension and creation tasks.

- **[Next-GPT (2023)](https://arxiv.org/abs/2309.05519)**  
  *Shengqiong Wu et al.*  
  **Key Insight**: Introduces an “any-to-any” multimodal LLM, offering flexible multimodal input-to-output mappings.

- **[Janus (2024)](https://arxiv.org/abs/2410.13848)**  
  *Chengyue Wu et al.*  
  **Key Insight**: Decouples visual encoding from the core architecture, simplifying the fusion of understanding and generation within a unified framework.

### AR is All You Need

- **[Emu3 (2024)](https://arxiv.org/abs/2409.18869)**  
  *Xinlong Wang et al.*  
  **Key Insight**: Argues that next-token prediction alone is sufficient, simplifying the paradigm for unified multimodal tasks.

- **[Chameleon (2024)](https://arxiv.org/abs/2405.09818)**  
  *Chameleon Team*  
  **Key Insight**: Employs mixed-modal early fusion and foundation model architectures to unify understanding and generation, driving simplicity and flexibility.

### AR + Diffusion/Flow Models

- *[Li, Tianhong et al. (2024)](https://arxiv.org/abs/2406.11838)*  
  **Key Insight**: Explores hybrid paradigms that leverage both autoregression and diffusion methods for integrated multimodal modeling.

- **[TransFusion (2024)](https://arxiv.org/abs/2408.11039)**  
  *Chunting Zhou et al.*  
  **Key Insight**: Combines autoregressive prediction and diffusion-based refinement, bridging understanding and generation at the token/image patch level.

- **[Show-O (2024)](https://arxiv.org/abs/2408.12528)**  
  *Jinheng Xie et al.*  
  **Key Insight**: Proposes a single transformer architecture that can handle both multimodal understanding and generation, emphasizing simplicity and scalability.

- **[JanusFlow (2024)](https://arxiv.org/abs/2411.07975)**  
  *Yiyang Ma et al.*  
  **Key Insight**: Integrates autoregression with rectified flows, enhancing the coherence and quality of multimodal outputs.

### Improved Tokenization

- **[TokenFlow (2024)](https://arxiv.org/abs/2412.03069)**  
  *Liao Qu et al.*  
  **Key Insight**: Develops a unified image tokenizer that brings image and language tokens closer together, enabling a single codebook for both understanding and generation.

---

## Contributions

We welcome contributions from the community! If you know of a relevant paper, model, or resource that’s missing, please:

- Submit a **Pull Request (PR)** with the new addition and a short summary.
- Open an **Issue** to propose new resources, categories, or improvements.

Recommended contributions include:

- Adding new papers (with a link and concise description).
- Updating existing entries (e.g., adding code repositories or related tutorials).
- Suggesting reorganizations or new categories to enhance discoverability and clarity.

---

## Logo Description

This logo was generated using **ChatGPT** in collaboration with the **DALL·E** model. It is specifically designed for the "Awesome Multimodal Understanding and Generation" repository, symbolizing the integration of text, images, and audio. The design features a modern, minimalistic flat style with clean geometric shapes and subtle gradients from blue to cyan, representing innovation, unity, and scalability.

**Prompt used for generation:**
A modern, minimalistic flat logo representing multimodal understanding and generation. The logo incorporates symbols of text, images, and audio, represented by geometric shapes such as a paragraph icon, a picture frame, and sound waves. The design uses a clean, geometric style with subtle gradients of blue and cyan, creating a sense of innovation, unity, and scalability. The background is white, ensuring the logo stands out clearly.



## License

This repository is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute its contents as permitted by the license.

---

**Happy exploring and contributing!**  
May this resource guide you in navigating and advancing the exciting landscape of unified multimodal models.
