```
Medical images are known to consume substantial amount of computational power due to their high resolutions, which restrict the application of deep learning in computation-constrained environment. We also observe that many types of medical images are spatially sparse. Therefore, by using standard dense implementation of convolutions, a lot of memory and computation is wasted on empty voxels, leading to low computation efficiency. However, computation efficiency has yet received adequate attention in medical image analysis. Improving the prediction accuracy is often the sole goal, neglecting the issues like high memory consumption and slow training.  Downsampling the images, dividing the images into smaller patches or extracting a bounding box of the region of interest are commonly used strategies for pre-processing high-resolution images. However, we show that these strategies are flawed and negatively affecting the results in some tasks like skull reconstruction.  We argue that it is beneficial to give the network a full-image context during training and the spatial sparsity of the medical images can be leveraged to reduce the memory consumption and speed up the training. 
```

## Sparse Convolutional Neural Networks for Medical Image Analysis

Check out the demonstration [**video**](https://www.techrxiv.org/articles/preprint/Sparse_Convolutional_Neural_Networks_for_Medical_Image_Analysis/19137518?file=34041689).

Full texts (preprint) including expeirments on other spatially sparse medical images can be found [**HERE**](https://www.techrxiv.org/articles/preprint/Sparse_Convolutional_Neural_Networks_for_Medical_Image_Analysis/19137518?file=34041698) (**Appendices C**).

**Our paper describes a practical solution to the curse of dimensionality in medical image analysis. The proposed approach is particularly relevant if your GPU memory does not possess the capacity to process the medical images at their original resolution and/or the sluggish training prohibits efficient hyper-parameter tunning. Our work describes the utility of sparse convolutions in shape completion, super-resolution and segmentation tasks. Experiments show that the proposed method is able to process high-resolution medical images using moderate memory and at a high speed.**


## skull shape completion and super-resolution
Thanks to [sparse convolutions](https://nvidia.github.io/MinkowskiEngine/overview.html), a deep neural net can be trained on full-resolution skull images (512x512xZ) for shape completion tasks. [Previous approaches](https://link.springer.com/book/10.1007%2F978-3-030-64327-0) use dense convolutions, so that the images have to be downsampled to fit in the GPU memory. A super-resolution network upsamples a coarse image to higher resolution (e.g., 512x512xZ) and restores its fine geometric details.

| shape completion (input-prediction-gt)|super-resolution (64-128-256-512)|
| ------      | ------ |
|[![skull shape completion](https://github.com/Jianningli/SparseCNN/blob/main/images/github1.png)] |  [![skull shape super-resolution](https://github.com/Jianningli/SparseCNN/blob/main/images/github2.png)]|



## medical image segmentation

Detailed workflow of using sparse neural nets in medical image **segmentation** can be found [here](https://www.techrxiv.org/articles/preprint/Sparse_Convolutional_Neural_Networks_for_Medical_Image_Analysis/19137518) (**Appendices C**).


| segmentation 1|segmentation 2|
| ------      | ------ |
|[![segmentation](https://github.com/Jianningli/SparseCNN/blob/main/images/github4.png)] |  [![segmentation](https://github.com/Jianningli/SparseCNN/blob/main/images/github5.png)]|




To cite our work:

```
@article{li2022sparsecnn,
  title={Sparse Convolutional Neural Networks for Medical Image Analysis},
  author={Li, Jianning and Gsaxner, Christina and Pepe, Antonio and Schmalstieg, Dieter and Kleesiek, Jens},
  journal={TechRxiv. Preprint.},
  year={2022}
}
```


