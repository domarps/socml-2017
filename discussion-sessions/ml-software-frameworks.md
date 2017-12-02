## Software Frameworks for Machine Learning

### `Tensorflow` vs `PyTorch`

#### TensorFlow
* Static graph (declarative)
* Good visualization using Tensor Board
* Easy for functional programmers
* Work in progress at Google to compile the models into binary
* Easy to use and deploy in GCP

#### PyTorch
* Ship the Lua RT
* Used in research
* Graph is dynamically constructed (imperative)
* Convenient for RNNs?

### ML pipelines - Is TF or PyTorch more friendly ?

* Distributed Learning

* Multi node training with TF
* Out of the box not great but needs augmentation tooling wise
* Steeper learning curve
* Synchronization step latency is a bottle neck

### MXNet 
- MXNet has a quicker learning and scales better as compared to TF as it uses parameter server (makes synchronization easier)
GPU Costs

### Other issues
- Storage Costs
- Distributed RL


## Addendum:
1. [Team Google Brain's view on PyTorch](https://www.reddit.com/r/MachineLearning/comments/6z51xb/we_are_the_google_brain_team_wed_love_to_answer/dmsqvej/)
2. [Roman Trusov's answer](https://www.quora.com/Is-Pytorch-better-than-Tensorflow-for-general-use-cases-1/answer/Roman-Trusov?srid=XoYJ)
3. [Hieu Pham's answer](https://www.quora.com/What-are-your-reviews-between-PyTorch-and-TensorFlow/answer/Hieu-Pham-20?srid=XoYJ)
