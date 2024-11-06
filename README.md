# FOIR-360 Task
# Abstract
Existing Salient Object Ranking (SOR) aims to infer ranking of salient objects based on their saliency degree. However, it tends to only focus on salient objects while neglecting non-salient ones. This coarse-grained ranking limits the
performance of downstream tasks. For instance, in image retrieval tasks, focusing solely on the relationship between salient objects is insufficient for achieving fine-grained scene analysis, which may result in retrieved results that do not satisfy user requirements. High-quality retrieval requires finegrained analysis, making it essential to rank non-salient objects. Based on this need, we propose a new task: Finegrained Object Importance Ranking in 360o Scenes (FOIR-
360), which focus on predicting the relative importance of “ALL objects” at the instance-level. Our task takes into account all objects, allowing us to refine the original “coarsegrained” to a “fine-grained” level. Currently, the main challenge for this new task is the lack of supervised data for model training or even for model testing. Therefore, we propose a novel weakly supervised method to address the shortage of datasets. Furthermore, to the best of our knowledge,
there is no existing suitable annotation protocol for this new task. The main reason is that annotating fine-grained rankings is extremely difficult, especially in panoramic scenes
that contain numerous instances where even humans are unable to determine which one is more important than others. As the first attempt, we introduce a new annotation protocol designed to highlight the ranking of objects that are nonsalient yet still important. Based on this protocol, we construct the first fine-grained 360Rank dataset. In summary, all these new task, weakly supervised method, annotation protocol, and dataset have the potential to drive advancements in the field. Both the code and dataset are publicly available at https://github.com/noname965/FOIR-360.
# Prerequisites
The training and testing experiments are conducted using PyTorch 1.10.0 with a single GeForce RTX 3090 GPU with 24GB Memory.
* Windows
* CUDA v11.1, cudnn v.7.5.0
* PyTorch 1.10.0
* torchvision
  
# 360Rank dataset

This repository provides the 360Rank dataset.
360Rank is a importance object ranking dataset of 500 images

### 

### Example

<div align=center><img src="./dataset.png"/></div>


## Download dataset
360Rank database can be downloaded from [BiaduPan](https://pan.baidu.com/s/1uqMPyqj4pznHZc7t4MYhKw)(key:hejz).

## TODO list
- [x] release the dataset [part1]
- [ ] release the dataset [part2]
- [ ] release the usuage code
