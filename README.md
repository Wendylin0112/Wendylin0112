<div align="center">

# Wei-Chen Lin 👋
### Computer Vision · Applied AI · Software Engineering

**Computer Science & Information Engineering Undergraduate**  
National Chung Cheng University, Taiwan

I build and evaluate computer vision systems, with an interest in turning research ideas into practical applications.

[![Profile Views](https://komarev.com/ghpvc/?username=Wendylin0112&label=Profile%20views&color=64748b&style=flat)](https://github.com/antonkomarev/github-profile-views-counter)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/wei-chen-lin-5487a135a/)
[![Email](https://img.shields.io/badge/Email-Contact-64748b?logo=gmail&logoColor=white)](mailto:iddw1498@gmail.com)

[Research](#-research) · [Projects](#-selected-projects) · [KNOWZAI](#-knowzai--disaster-resilience-in-practice) · [Community](#-community--leadership) · [Resume](#-resume) · [Contact](#-contact)

</div>

---

## 👋 About Me

I'm a CSIE undergraduate at **National Chung Cheng University (CCU)**, having transferred from Mathematics. I enjoy translating abstract ideas into working systems—and investigating their reliability through experiments, evaluation, and iteration.

My interests center on **computer vision**, **machine learning**, and **practical AI development**. Alongside my technical work, I have led interdisciplinary software collaborations and helped build an early-stage disaster-preparedness product. I also enjoy discrete mathematics, graph algorithms, and logic through coursework and personal exploration.

## 🔬 Research

### 360° Multi-Camera Person Re-Identification & Tracking · Ongoing

**Undergraduate research · RockCore industry collaboration · Advisor: Prof. Wei-Yang Lin**

**Problem:** How can a tracking system maintain consistent identities as people move across multiple panoramic cameras, despite viewpoint changes, distortion, and look-alike appearances?

**My work:** Contributed to person-detection/tracking and ReID pipeline integration; compared OSNet, TransReID, and CLIP-ReID on preliminary data; prepared ground-truth annotations for HOTA evaluation; and explored face/body feature fusion and one-to-one global identity association.

**Current focus:** More rigorous evaluation and reliable identity matching rather than relying only on promising baseline scores.

[Read the public research overview](./research/360-multicamera-reid.md) · *Collaborative code repository is private; unpublished code and data are not publicly available.*

### Acute Appendicitis Analysis via U-Net-Based CT Segmentation

**Graduate-level medical-image-analysis course project · MATLAB · Team Honorable Mention**

**Problem:** Explore whether CT image segmentation can support scan-level acute-appendicitis classification.

**My contribution:** Built the **2D U-Net branch**, including preprocessing, data augmentation, custom Dice loss, and probability/area-threshold post-processing. A senior collaborator separately implemented the **nnU-Net branch**, maintained in her own repository.

**Result:** **Scan-level F1 = 0.833** for my 2D U-Net branch on a course-provided **20-patient evaluation set**; the separate nnU-Net branch achieved about **0.667**. These are limited course-project results, not independently validated clinical performance.

[My 2D U-Net code & report](https://github.com/Wendylin0112/AOCR2024-AI-Challenge) · [Collaborator's nnU-Net](https://github.com/zihyuhe/nnU-Net-med-img) · [Team poster (PDF)](https://github.com/Wendylin0112/AOCR2024-AI-Challenge/blob/main/%E9%86%AB%E5%AD%B8%E5%BD%B1%E5%83%8Fproject%E5%A3%81%E5%A0%B1%E5%BD%B1%E5%8D%B0%E7%89%88%E6%9C%AC.pdf)

## 🚀 Selected Projects

### 1. Trustworthy AI Assessment System

**Team leadership · Requirements engineering · LLM-assisted evaluation**

An eight-member international software engineering project to help users assess AI systems across **11 trustworthiness indicators** through lifecycle questionnaires, weighted scores, radar visualizations, and generated reports.

**My contribution:** As project leader, coordinated stakeholder requirements, team responsibilities, schedules, integration and progress presentations. I also worked on questionnaire content, LLM-assisted report workflows, PDF output testing and deployment support.

**Outcome:** An integrated assessment platform with a documented end-to-end system demonstration.

[Frontend & documentation](https://github.com/TAI-trustworthy-ai-lab/Trustworthy-AI-Assessment-System-Design) · [Backend](https://github.com/TAI-trustworthy-ai-lab/backend) · **[Watch system demo](https://www.youtube.com/watch?v=jxtBbBmE0rw)** · [Technical presentation (PDF)](https://github.com/TAI-trustworthy-ai-lab/Trustworthy-AI-Assessment-System-Design/blob/main/docs/FinalProjectPresentation.pdf)

[![TAI assessment platform — video walkthrough](https://img.youtube.com/vi/jxtBbBmE0rw/hqdefault.jpg)](https://www.youtube.com/watch?v=jxtBbBmE0rw)

<sub>Video walkthrough: indicator prioritization, questionnaire flow, and visualization of assessment results.</sub>

### 2. My CCU Academia — LLM-Powered Campus RPG

**Python · Llama 3.2 · Ollama · Flask · Unity**

A 2D pixel RPG inspired by CCU campus life, with AI-powered NPC conversations built from community discussion content.

**My contribution:** Proposed the LLM-NPC concept and worked on data collection, character/personality processing, multi-turn dialogue handling, and REST API integration with Unity.

**Outcome:** A playable browser-hosted game built by a three-person team. Some AI dialogue functionality may depend on separate services.

**[Play the game](https://play.unity.com/en/games/0b839150-5aed-4c84-affa-60d44727fdbf/ccuacademia)** · [Source repository](https://github.com/Eijiro1016/CCU_Academia)

### 3. Power-Line Asset Defect Classification

**PyTorch · EfficientNet-B0 · Streamlit**

A two-stage inspection-image pipeline that first identifies one of **five equipment categories**, then chooses a global or category-specific defect classifier.

**My work:** Developed model training and threshold adjustment workflows and made predictions accessible through a Streamlit interface.

**Result:** The repository reports **F1 = 0.8975**, **precision = 0.9206**, and **recall = 0.8756** for its selected final submission; these figures refer to the project's reported evaluation, not independent field validation.

**[Try the Streamlit demo](https://datamining-finalproject-jwxzxr4njtsox4z9quebt7.streamlit.app/)** · [Source, methods & results](https://github.com/Wendylin0112/DataMining-FinalProject)

<sub>Demo allows image upload, component predictions, defect scores, and CSV export. Hosted demos may require a short startup period.</sub>

### 4. Kidney Microvascular Segmentation

**Individual medical imaging coursework · MATLAB · 2D U-Net**

Explored vessel segmentation on PAS-stained kidney histology tiles, including polygon-to-mask conversion, augmentation, training, and visualization. The experiment highlighted class imbalance and why aggregate accuracy alone can be misleading.

[Technical case study & limitations](./projects/kidney-microvascular-segmentation.md)

### More Projects

- **[Shortest-Path Optimization](https://github.com/Wendylin0112/shortest-path-competition)** — C++17, Dijkstra, ALT/A*; [optimization benchmark](https://github.com/Wendylin0112/shortest-path-competition/blob/main/optimization_report.md).
- **[Hand-Control Runner](https://github.com/Wendylin0112/Hand-Control-Runner)** — MATLAB + MediaPipe gesture-controlled games; [watch the demo](https://youtu.be/FydK0xX9bpE).

## 🌏 KNOWZAI — Disaster Resilience in Practice

**Early-stage interdisciplinary startup team · Technical development · MVP completed**

We're building **KNOWZAI (攏災影)**, an integrated disaster-preparedness and response app. The MVP brings together disaster information, map-based reporting, and location-related features, with AI-assisted guidance in our broader product direction.

Our team is currently working on **field validation and requirements discovery**. I'm involved primarily in technical development, turning product needs into a working prototype.

Interested in learning more, collaborating, or joining the team? **We welcome conversations with people who care about disaster resilience and practical technology.**

**[Official website](https://knowzai-web.vercel.app/)** · [Team GitHub](https://github.com/long-tsai-iann) · [Team presentation](https://canva.link/z9eoxrgxywhuqrz)

**Team contact:** [longtsaiiann@gmail.com](mailto:longtsaiiann@gmail.com)

## 🛠️ Technical Skills

**Languages:** Python · C/C++ · MATLAB · Java · C# · R  
**AI / Computer Vision:** PyTorch · scikit-learn · Image segmentation · Person ReID · Object tracking  
**Software & Tools:** Git/GitHub · Linux · Docker · Flask · Next.js/React · Node.js/Express · PostgreSQL · Streamlit

## 🤝 Community & Leadership

- **MATLAB Student Ambassador (MathWorks):** Organized hands-on campus learning events and promoted MATLAB learning resources. [Awesome MATLAB Students](https://github.com/mathworks/awesome-matlab-students).
- **Vice Captain, CCU Competitive Programming Club:** Coordinated activities, student outreach, and club operations.
- **Teaching Assistant, CCU:** Supported instruction, grading, and student troubleshooting, including assessment-preparation tooling.

## 📄 Resume

**[View my online resume](./RESUME.md)** — a concise overview of education, research, projects, and leadership experience.

## 📫 Contact

**Email:** [iddw1498@gmail.com](mailto:iddw1498@gmail.com) · **LinkedIn:** [Wei-Chen Lin](https://www.linkedin.com/in/wei-chen-lin-5487a135a/) · **GitHub:** [Wendylin0112](https://github.com/Wendylin0112)

For KNOWZAI team inquiries: **[longtsaiiann@gmail.com](mailto:longtsaiiann@gmail.com)**.

---

<div align="center"><sub>Research-minded engineering · Practical AI · Collaborative problem solving</sub></div>
