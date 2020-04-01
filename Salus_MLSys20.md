# Fine-Grained GPU Sharing Primitives for Deep Learning Applications. In MLSys'20.
# Summary
Based on the current coarse GPU sharing technologies (the minimum unit >= 1 GPU card), deep learning frameworks cannot utilize GPU resources fully (GPU underutilization) when training multiple deep learning models concurrently. To resolve this, they proposed Salus ... In summary, their contributions are three-fold: 1) they identified the importance of fine-grained GPU sharing methods; 2) they proposed a plausible solution named Salus based on fast job switching and memory sharing; 3) Extensive experiments.
# Evaluation
# Conclusion
From my perspective, this paper is like an workshop paper because they attract many researchers' attention on **scheduling algorithms on fine-grained GPU sharing primitives** but they haven't provided the optimization. Besides, efficient scheduling algorithms on fine-grained GPU are useful to the current edge computing or other resource-constrained environments.
