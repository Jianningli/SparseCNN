## Sparse Convolutional Neural Networks for Medical Image Analysis

Full texts including expeirments on other spatially sparse medical images can be found [here](https://www.techrxiv.org/articles/preprint/Sparse_Convolutional_Neural_Networks_for_Medical_Image_Analysis/19137518) (**Appendices C**)

**Our work describes a practical solution to the curse of dimensionality in medical image analysis. The proposed approach is particularly relevant if your GPU memory does not possess the capacity to process the medical images at their original resolution and/or the sluggish training prohibits efficient hyper-parameter tunning. Our work describes the utility of sparse convolutions in shape completion, super-resolution and segmentation tasks. **


## skull shape completion and super-resolution
thanks to the [sparse convolutions](https://nvidia.github.io/MinkowskiEngine/overview.html), the skull images can be trained at their full resolution (512x512xZ) for shape completion tasks. A super-resolution networt upsamples a coarse image to higher resolution (e.g., 512x512xZ) and restores its fine geometric details.

| shape completion (input-prediction-gt)|super-resolution (64-128-256-512)|
| ------      | ------ |
|[![Studierfenster](https://github.com/Jianningli/SparseCNN/blob/main/images/github1.png)] |  [![Skull Shape Reconstruction](https://github.com/Jianningli/SparseCNN/blob/main/images/github2.png)]|



## medical image segmentation







































```Python
@article{li2022sparsecnn,
  title={Sparse Convolutional Neural Networks for Medical Image Analysis},
  author={Li, Jianning and Gsaxner, Christina and Pepe, Antonio and Schmalstieg, Dieter and Kleesiek, Jens},
  journal={TechRxiv. Preprint.},
  year={2022}
}
```


