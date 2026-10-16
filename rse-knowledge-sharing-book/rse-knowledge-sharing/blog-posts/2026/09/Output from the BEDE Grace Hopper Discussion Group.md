# Output from the BEDE Grace Hopper Discussion Group Workshop

An online drop in session for users of the Grace hoppers was held in March. This was attended by GH users from across the UK including N8 institutions. We compared the GHs with similar hardware and identified some of the challenges and solutions to getting the most out of the hardware. The attendees were a mix of those that had used the GHs and some who were interested to know if it was a good solution for their project.

We discussed how among other things the GH architecture could be used for Agent based modelling, training generative AI on 3d imagery and other pytorch related uses for Machine Learning models.

The main challenge highlighted in optimizing for the GH architecture was managing the unified memory across GPU and CPU. It was however agreed that it has been easier to port software to the GHs than to the Power 9s as there are less architecture specific compiler issues. It was also highlighted that many issues were overcome once the underlying libraries had been ported to the hardware and that many providers had now updated packages to support the GH architecture.

One barrier to making the most of the GH architecture was the lack of specific funding to optimize especially for this hardware.

Another challenge was the difference between arm and x86 systems with some subtle compiler differences that could cause issues. The main difference being char being signed or unsigned.

Despite the challenges in porting code most users had seen significant performance improvements. This supports the benchmarking previously performed by Sheffield.

Alternatives to GH architecture were discussed including the issue of the cost of Grace Hoppers. Some institutions are looking into AMD options. The biggest attraction of the GHs is the amount of memory.

The group agreed that some training on the use of unified memory may be beneficial and resources were shared on [documentation on its use](https://docs.nvidia.com/cuda/cuda-programming-guide/04-special-topics/unified-memory.html). It was suggested that these should focus on a particular use case or software such as Pytorch.
