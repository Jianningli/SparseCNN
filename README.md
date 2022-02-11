## Sparse Convolutional Neural Networks for Medical Image Analysis

Full texts including expeirments on other spatially sparse medical images can be found [here](https://www.techrxiv.org/articles/preprint/Sparse_Convolutional_Neural_Networks_for_Medical_Image_Analysis/19137518) (**Appendices C**)




## skull shape completion and super-resolution
thanks to the [sparse convolutions](https://nvidia.github.io/MinkowskiEngine/overview.html), the skull images can be trained at their full resolution (512*512*Z) for shape completion tasks. A super-resolution networ upsample a coarse image to higher resolution (e.g., 512*512*Z) and restore fine geometric details.

| shape completion|super-resolution|
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


