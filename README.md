# SPARTAN: Sparse Hierarchical Memory for Parameter-Efficient Transformers

<!-- <img src="Resources/Spartan_BERT_Logo.png"/> -->
<img src="Resources/Spartan_BERT_Logo.png" width="50" align="center"/>

Code for the paper titled: SPARTAN: Sparse Hierarchical Memory for Parameter-Efficient Transformers [[Paper]]()

### Description

##### Pictorial representation
<img src="Resources/Teaser_with_caption.png"/>

##### Abstract
Fine-tuning pre-trained language models (PLMs) achieves impressive performance on a range of downstream tasks, and their sizes have consequently been getting bigger. Since a different copy of the model is required for each task, this paradigm is infeasible for storage-constrained edge devices like mobile phones. In this paper, we propose SPARTAN, a parameter efficient (PE) and computationally fast architecture for edge devices that adds hierarchically organized sparse memory after each Transformer layer. SPARTAN freezes the PLM parameters and fine-tunes only its memory, thus significantly reducing storage costs by re-using the PLM backbone for different tasks. SPARTAN contains two levels of memory, with only a sparse subset of parents being chosen in the first level for each input, and children cells corresponding to those parents being used to compute an output representation. This sparsity combined with other architecture optimizations improves SPARTAN's throughput by over `90%` during inference on a Raspberry Pi 4 when compared to PE baselines (adapters) while also outperforming the latter by `0.1` points on the GLUE benchmark. Further, it can be \textit{trained} `34%` faster in a few-shot setting, while performing within `0.9` points of adapters. Qualitative analysis shows that different parent cells in SPARTAN specialize in different topics, thus dividing responsibility efficiently.

### Installation instruction

`Step 0`: We recommend creating a `conda` environment
``` bash
conda create -n spartan python=3.8
```

`Step 1`: Install the requirements
``` bash
pip install -r requirements.txt
```

`Step 2`: Setup the SPARTAN package
``` bash
pip install .
```

### Citation
Please use the following citation if you found the paper useful!

```
Will be released soon!
```