Research notes and code for AI-Systems.
# AI-Systems
With developments of big data, big systems and large open-source AI frameworks, many researchers are interested in build AI-Systems. Combined with many system's concerns, AI-systems have four research challenges: 
1. Mission-critical AI (Design AI Systems that learn continually by interacting with a dynamic environment, while making decision that are timely, robust and secure).
2. Personalized AI (Design AI Systems that enable personalized applications and services yet do not compromise user's privacy and security).
3. AI across organizations (Design AI Systems that can train on datasets owned by different organizations without compromising their confidentiality, and in the process provide AI capabilities that span the boundaries of potentially competing organization).
4. AI demands outpucing the Moore's Law (Develop domain-specific architectures and software systems to address the performance needs of future AI applications in the post-Moore's Law era, including custom chips for AI work-loads, edge-cloud systems to efficiently process data at the edge, and techniques for abstracting and sampling data).
In the four challenges, [1] proposed nine research opportunites: 1) Continual learning; 2) Robust decision; 3) Explainable decision; 4) Secure enclaves; 5) Adversarial learning; 6) Sharing learning on confidential data; 7) AI-specific architecturesl; 8) Composable AI systems;9) Cloud-edge systems. <br>
I arrange AI-sys papers in these nine categories as follows and put classic AI papers in the first subsection.<br>

[1] [Stoica et al. A Berkeley View of Systems Challenges for AI.](https://arxiv.org/pdf/1712.05855.pdf)
## Classic AI-models
## Continual learning
1. Build systems for RL that fully exploit parallelism, while allowing dynamic task graphs, providing millisecond-level la- tencies, and running on heterogeneous hardware under stringent deadlines.
2. Build systems that can faithfully simulate the real-world environment, as the environment changes continually and unexpect- edly, and run faster than real time.
## Robust decision
1. Build fine grained provenance support into AI sys- tems to connect outcome changes (e.g., reward or state) to the data sources that caused these changes, and automatically learn causal, source-specific noise models.
2. Design API and language support for developing systems that maintain confidence intervals for decision- making, and in particular can flag unforeseen inputs.
## Explainable decision
Build AI systems that can support interactive diagnostic analysis, that faithfully replay past executions, and that can help to determine the features of the input that are responsible for a particular decision, possibly by replaying the decision task against past perturbed inputs. More generally, provide systems support for causal inference.
## Secure enclaves
Build AI systems that leverage secure enclaves to ensure data confidentiality, user privacy and decision integrity, possibly by splitting the AI system’s code between a minimal code base running within the enclave, and code running outside the enclave. Ensure the code inside the enclave does not leak information, or compromise decision integrity.
## Adversarial learning
Build AI systems that are robust against adversarial inputs both during training and prediction (e.g., decision making), possibly by designing new machine learning models and network architectures, leveraging provenance to track down fraudulent data sources, and replaying to redo decisions after eliminating the fraudu- lent sources.
## Sharing learning on confidential data
1. Build AI systems that can learn across multiple data sources without leaking information from a data source during training or serving.
2. Build AI systems that provide incentives to potentially competing organizations to share their data or models.
## AI-specific architectures
1. Design domain-specific hardware architectures to improve the performance and reduce power consumption of AI ap- plications by orders of magnitude, or enhance the security of these applications.
2. Design AI software systems to take advantage of these domain-specific architectures, resource disaggregation architectures, and future non-volatile storage technologies.
## Composable AI systems
Design AI systems and APIs that allow the composition of models and actions in a modular and flexible manner, and develop rich libraries of models and options using these APIs to dramatically simplify the development of AI applications.
## Cloud-edge systems
1. Design cloud-edge AI systems that leverage the edge to reduce latency, improve safety and security, and implement intel- ligent data retention techniques.
2. Design cloud-edge AI systems that leverage the cloud to share data and models across edge devices, train sophisticated computation- intensive models, and take high quality decisions.
# Useful external Resources
## Course
1. [CSE 599W: Systems for ML](http://dlsys.cs.washington.edu/)
2. [AI-Sys: Machine Learning Systems](https://ucbrise.github.io/cs294-ai-sys-fa19/#today)
## Conference
1. [SysML: Systems and Machine Learning](https://mlsys.org/Conferences/2019/index.html#body)
