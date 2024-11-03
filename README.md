# 3D-Anatomy-Reconstruction
In recent years, remarkable advancements have been achieved in
computer vision, particularly in the reconstruction of
two-dimensional (2D) images depicting various scenes, objects,
and environments. However, transitioning from 2D image
reconstruction to three-dimensional (3D) image reconstruction
poses a significant challenge.

Our focus is on reconstructing missing anatomical structures
within a human body based on a given 3D anatomy. This concept
finds its inspiration in various biological conditions or traumatic
incidents that can result in underdeveloped or absent organs in
the human body. Whether due to mutations during birth,
inadequate nutrition and diet, accidents, or traumatic injuries, all
these factors may contribute to an underdeveloped human body.

The objective of our project is to develop a deep learning model
capable of taking 3D scanned images of cross-sections of the
human body in medical image formats as input and producing a
reconstructed version of the image as output.

The inherent challenge lies in the fact that research in this specific
field is still ongoing, with only a few selective deep learning
models and papers focusing on 3D images.

We have made a deep learning model for 3d anatomy reconstruction, where we leveraged the use cases of 3D Unet with skip connections/ GoogleNet.

| Overview       | Details |
| -------------- | ------- |
| **Title**      | 3D Anatomy Reconstruction |
| **Link to paper** | [Paper](https://arxiv.org/abs/2309.04956) |
| **Benchmark**  | Multi-class Anatomy Completor |
| **Link to benchmark dataset** | [Download (multi-class)](https://files.icg.tugraz.at/f/b0623306eb9246be8c3c/?dl=1) |
| **Data structure** | voxel occupancy grid |
| **Pretrained Model** | [Model](https://drive.google.com/drive/folders/15iy86nhCFKLpnIPgxniZjJqspSbZv3Ub?usp=drive_link ) |

## To run the training Code for Unet

1. Navigate to the `Unet` directory:
    ```sh
    cd Unet
    ```
2. Run the `code.ipynb` file.

## Results from the Unet

![Result from UNET where left is incomplete image and right one is complete one](https://github.com/krishmittal1301/3D-anatomy-completer-/blob/main/Unet/WhatsApp%20Image%202024-05-07%20at%2010.55.53_28ebe640.jpg)
**Figure: Result from UNET where the left is the complete image and the right one is the incomplete one.**

## Similarly we can run the code for skip connections and GoogleNet.

![Result from UNET where left is incomplete image and right one is complete one](https://github.com/krishmittal1301/3D-anatomy-completer-/blob/main/Unet%2BSkip/WhatsApp%20Image%202024-05-14%20at%2016.10.08_2b9a161b.jpg)
**Figure: Result from GoogleNet+Skip connections. The left is the incomplete image and the right one is the complete one.**

## Loss Comparison of all the models

![Result](https://github.com/Techtronics21/3D-anatomy-reconstruction/blob/main/Loss_comparison.png)

**Figure: Results indicate that GoogleNet + Skip connections was the best suited model**
