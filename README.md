Research notes and codes for AI-Systems. Since I'm interested in building and deploying intelligent video-based applications, I will take notes for intelligent video systems carefully. But for other AI systems, I only summarize their problems.
# AI-Systems
As discussed in [1, 2], there are three system-level concerns in real-world AI applications. They are deployment, cost and accessibility. 

[1] [Stoica et al. A Berkeley View of Systems Challenges for AI.](https://arxiv.org/pdf/1712.05855.pdf)<br>
[2] [Ratner et al. MLSys: The New Frontier of Machine Learning Systems.](https://arxiv.org/abs/1904.03257)

## Deployment Concerns
Deployment concerns include **robustness** to adversarial influences or other spurious factors; safety more broadly considered; **privacy** and security, especially as sensitive data is increasingly used; **interpretability**, as is increasingly both legally and operationally required; **fairness**, as ML algorithms begin to have major effects on our everyday lives; and many other similar concerns.<br>
###### Video
[1] [Cryptography for Safe Machine Learning. In MLSys'20.](https://www.youtube.com/watch?v=VlfZ7-5bKqk): [Shafi Goldwasser](https://simons.berkeley.edu/people/shafi-goldwasser) presented some techniques about cryptography in machine learning.
###### Paper
[1] [Telekine: Secure Computing with Cloud GPUs. In NSDI'20.](https://www.usenix.org/conference/nsdi20/presentation/hunt): they aim to solve some concerns about **privacy** in the recent GPU trusted execution environments (TEE). <br>
[2] [Themis: Fair and Efficient GPU Cluster Scheduling. In NSDI'20.](https://www.usenix.org/conference/nsdi20/presentation/mahajan): a **fair** GPU scheduling algorithm.
## Cost
Cost on annotation, computation, latency and power. <br>
### Video
[1] [Theory & Systems for Weak Supervision. In MLSys'20.](https://www.youtube.com/watch?v=CR1g2-ZqswE): [Christopher Ré](https://cs.stanford.edu/people/chrismre/) highlighted the importance of **data** in the real world deployments because we aren't usually able to get enough high quality labels for large training data. To bride this gap, he introduced many works from theoretical analysis to real world deployment about weak supervised learning, which only learns from noisy weakly labels. Also, He introduced [Snorkel](https://www.snorkel.org/) which is a popular weak supervised framework developed by Brown University.
### Paper
[1] [Improving Resource Efficiency of Deep Activity Recognition via Redundancy Reduction. In HotMobile'20.](https://dl.acm.org/doi/abs/10.1145/3376897.3377859): they target to reduce cost on **computation and memory** of deep human activity recognition (HAR) models. [Note](https://github.com/YanLu-nyu/Awesome-AI-Systems/blob/master/HAR_HotMobile_20.md)
## Accessibility
Accessibility to developers and organizations without PhD-level machine learning and systems expertise.
### Paper
[1] [A System for Massively Parallel Hyperparameter Tuning. In MLSys'20.](https://proceedings.mlsys.org/static/paper_files/mlsys/2020/94-Paper.pdf): they proposed a new hyperparameter optimization algorithm named ASHA to solve large-scale hyperparameter optimization problems in distributed training.
# Useful external Resources
## Books for Deep Learning (a popular learning approaches in machine learning)
1. [Dive into Deep Learning](http://d2l.ai/chapter_linear-networks/index.html)
2. [Deep Learning](http://www.deeplearningbook.org/)
## Course
1. [CSE 599W: Systems for ML](http://dlsys.cs.washington.edu/): Low-level optimization in Deep Learning frameworks.
2. [AI-Sys: Machine Learning Systems](https://ucbrise.github.io/cs294-ai-sys-fa19/#today)
## Conference
1. [SysML: Systems and Machine Learning](https://mlsys.org/Conferences/2019/index.html#body)
2. [SOSP: ACM Symposium on Operating Systems Principles](https://sosp19.rcs.uwaterloo.ca/program.html)
3. [OSDI: USENIX Symposium on Operating Systems Design and Implementation](https://www.usenix.org/conference/osdi18)
## Tools
1. [TVM: End to End Deep Learning Compiler Stack](https://tvm.apache.org/)
