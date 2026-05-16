Title: DeltaTokens: 100× Token-Efficient Video
Representation for World Models

Qiang Zhang (https://www.linkedin.com/in/qiang-zhang-6b48791a7/)

Abstract:
Video generation models have demonstrated remarkable potential for applications ranging from filmmaking and advertising to humanoid robot world modeling.
However, current systems suffer from several fundamental bottlenecks: prohibitively high training and inference costs, and limited generation length, typically constrained to short video clips.
We argue that these limitations largely stem from inefficient video representations, particularly those based on conventional Video VAEs. Existing Video VAEs often require more than 10k tokens per second of high-quality video, resulting in extremely long token sequences for downstream transformer models, whose computational cost scales quadratically with sequence length.
In this paper, we introduce DeltaTokens, a novel and highly efficient video representation that achieves comparable reconstruction quality while using up to 100× fewer tokens. DeltaTokens is built upon a causal, streaming encoder that compactly encodes inter-frame delta information (motion) into one-dimensional token sequences, paired with a causal streaming decoder and a diffusion-based decoder to reconstruct high-fidelity videos.
Extensive experiments demonstrate that DeltaTokens significantly improves both reconstruction efficiency and generation scalability, enabling longer video generation at substantially reduced computational cost. Our results suggest that rethinking video representations through delta-based tokenization is a promising direction for scalable video generation models. 

video1: https://deltatokenproj.sfo3.cdn.digitaloceanspaces.com/presentation/content_demo_0430.mp4
video2: https://deltatokenproj.sfo3.cdn.digitaloceanspaces.com/presentation/robot_demo_0430.mp4