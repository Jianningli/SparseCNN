<div align="center">
  <h1>Sparse Convolutional Neural Network for High-Resolution Skull Shape Completion and Shape Super-Resolution</h1>
  
  <p>
    <a href="https://www.nature.com/articles/s41598-023-47437-6"><img src="https://img.shields.io/badge/Nature_Scientific_Reports-Paper-B31B1B?style=flat-square&logo=springer&logoColor=white" alt="Paper" /></a>
    <a href="https://dl.dropboxusercontent.com/s/2cit5cue7e1u557/notes.txt?dl=0"><img src="https://img.shields.io/badge/Motivation-Letter-0078D4?style=flat-square&logo=dropbox&logoColor=white" alt="Motivation Letter" /></a>
    <a href="https://www.techrxiv.org/articles/preprint/Sparse_Convolutional_Neural_Networks_for_Medical_Image_Analysis/19137518?file=34041689"><img src="https://img.shields.io/badge/Demo-Video-FF0000?style=flat-square&logo=youtube&logoColor=white" alt="Video" /></a>
  </p>
</div>

> **Our paper describes a practical solution to the curse of dimensionality in medical image analysis.** The proposed approach is particularly relevant if your GPU memory does not possess the capacity to process the medical images at their original resolution and/or sluggish training prohibits efficient hyper-parameter tuning. Our work describes the utility of sparse convolutions in shape completion, super-resolution, and segmentation tasks. Experiments show that the proposed method can process high-resolution medical images using moderate memory and at a high speed.

---

## 💀 Skull Shape Completion and Super-Resolution

Thanks to [sparse convolutions](https://nvidia.github.io/MinkowskiEngine/overview.html), a deep neural network can be trained on full-resolution skull images (512x512xZ) for shape completion and shape super-resolution tasks. 

[Previous approaches](https://ieeexplore.ieee.org/document/9420655) (or [this](https://www.sciencedirect.com/science/article/abs/pii/S1361841523001251)) use dense convolutions, meaning images have to be downsampled to fit into GPU memory. A super-resolution network upsamples a coarse image to a higher resolution (e.g., 512x512xZ) and restores its fine geometric details on the shape surface.

| Shape Completion (Input - Prediction - GT) | Super-Resolution (64 - 128 - 256 - 512) |
| :---: | :---: |
| <img src="https://github.com/Jianningli/SparseCNN/blob/main/images/github1.png" alt="skull shape completion" width="400"/> | <img src="https://github.com/Jianningli/SparseCNN/blob/main/images/github2.png" alt="skull shape super-resolution" width="400"/> |

---

## 🩻 Medical Image Segmentation

A detailed workflow of using sparse neural nets in medical image **segmentation** can be found [here](https://static-content.springer.com/esm/art%3A10.1038%2Fs41598-023-47437-6/MediaObjects/41598_2023_47437_MOESM1_ESM.pdf).

| Segmentation 1 | Segmentation 2 |
| :---: | :---: |
| <img src="https://github.com/Jianningli/SparseCNN/blob/main/images/github4.png" alt="segmentation 1" width="400"/> | <img src="https://github.com/Jianningli/SparseCNN/blob/main/images/github5.png" alt="segmentation 2" width="400"/> |

---

## 📝 Citation

If you find this work useful, please cite:

```bibtex
@article{li2023sparse,
  title={Sparse Convolutional Neural Network for High-resolution Skull Shape Completion and Shape Super-resolution},
  author={Li, Jianning and Gsaxner, Christina and Pepe, Antonio and Schmalstieg, Dieter and Kleesiek, Jens and Egger, Jan},
  journal={Scientific Reports},
  volume={13},
  doi={https://doi.org/10.1038/s41598-023-47437-6},
  year={2023}
}
```
