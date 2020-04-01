# Fine-Grained GPU Sharing Primitives for Deep Learning Applications. In MLSys'20.
# Summary
Based on the current coarse GPU sharing technologies (the minimum unit >= 1 GPU card), deep learning frameworks cannot utilize GPU resources fully (GPU underutilization) when training multiple deep learning models concurrently. To resolve this, they designed and implemented Salus adaptor between deep learning framework and the hardware as presented in _Figure 3_.
![](https://github.com/YanLu-nyu/Awesome-AI-Systems/blob/master/Salus_design.png)<br>
Salus consists two key characteristics: 1) keep persistent memory (framework and model) during the training to accelerate job switching; 2) use GPU lane to control the GPU memory usage of different deep learning workloads. Based on the two primitives, they tested four different scheduling approaches and found that **SRTF** performed the best. In summary, their contributions are three-fold: 1) they identified the importance of fine-grained GPU sharing methods; 2) they proposed a plausible solution named Salus based on fast job switching and memory sharing; 3) Extensive experiments.
# Evaluation
They test different common scheduling algorithms on Salus:
1. **FIFO**: refers to processing jobs in order of their arrival.
2. **SRTF**: is a preemptive shortest-remaining-time-first scheduler. They assume that the duration is known or can be estimated.
3. **PACK**: attempts to pack as many jobs as possible in to the GPU.
4. **FAIR**: uses time sharing to equally share the GPU time among many jobs.
# Conclusion
From my perspective, this paper is like an workshop paper because they attract many researchers' attention on **scheduling algorithms on fine-grained GPU sharing primitives** but they haven't provided the optimization. Besides, efficient scheduling algorithms on fine-grained GPU are useful to the current edge computing or other resource-constrained environments.
