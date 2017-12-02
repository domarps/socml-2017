## Future of Hardware for Deep Learning

### Nvidia GPU roadmap
* Depends on application class.
* Inference for IoT - Things that require low power will end up running on fixed function ASICs.
* Inference for Cloud - Increased specialization in GPUs (optimized for specific operations by having exclusive instructions)
* Deep Learning Accelerator - OpS TPU from Nvidia
* Sparsity
* Different layers of a network needs different dynamic ranges
* Hardware for training vs inference. Latter has much less memory requirement (no need to keep around all weights and activations in case of inference)
* ASICs are specialized for a class of models

### Biologically Inspired Architectures (BICA)
* Neuromorphic architectures (viz. Numenta, Vicarious Systems)
* Generic models but not very accurate - but how is this more generic than TPUs ? 2D vs 3D architecture (brain is 3D and async in computation). Even if we understood the brain does it make sense to build hardware to mimic the brain ?
* Activation vs Inhibition ? Brain is always active and it inhibits selectively. But inhibition is just negative weights.

### Startups in DL hardware
* Graphcore - Maybe training chip ?

### Alternative to GPUs
* No specialized instructions for tensor ops
* Edge Node HW
* Tegra from NVIDIA
* Raspberry Pi can run some deep learning architectures

### Rants
* GPU frustrations
* CUDA driver installation is still a pain (although AWS and other cloud vendors make it easier)
* How does one educate oneself on GPU tricks ?
* Alternative to CUDA - OpenCL, RockAM (not as performant)

