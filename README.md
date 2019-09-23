# Illumination-guided Neural Style Transfer

This method is able to generate fine artworks for the following subjects:
* 3D models which include a digital real-world scene or an object;
* 2D photos which contain a lot of sunlight or complex lighting conditions, such as lanscapes, sky, natural objects, and etc.

This method can preserve the illumination and scene structure of the input photos, during the process of neural style transfer.

## Requirements

* python 3
* pytorch 1.0+
* matlab

## Getting Started

* Photo images and style images: "/inputs/inputs/"
* Illumination maps:  "/inputs/inputs_semlight/"
* output artworks (there are some results examples in it): "/outputs/STYLE_NAME/"
* codes in the folder "/IIumination_matlab/" are used for calculating illumination maps
* codes in the folder "/image_analogy/" are models and losses used for illumination-guided neural style transfer, built upon [neural image analogies](https://github.com/awentzonline/image-analogies) by Adam Wentz.
* main function: "/scripts/main.py"

## References

1. Fišer, Jakub, et al. **StyLit: illumination-guided example-based stylization of 3D renderings**. ACM Transactions on Graphics (TOG) 35.4 (2016): 92. [StyLit](https://dl.acm.org/citation.cfm?id=2925948)
2. Gatys, Leon A., Alexander S. Ecker, and Matthias Bethge. **Image style transfer using convolutional neural networks**. Proceedings of the IEEE conference on computer vision and pattern recognition. 2016. [Neural Style Transfer](http://openaccess.thecvf.com/content_cvpr_2016/html/Gatys_Image_Style_Transfer_CVPR_2016_paper.html)
3. Liao, Jing, et al. **Visual attribute transfer through deep image analogy**. ACM Transactions on Graphics (TOG) 36.4 (2017): 120. [Deep Image Analogy](https://arxiv.org/abs/1705.01088)
4. Champandard, Alex J. **Semantic style transfer and turning two-bit doodles into fine artworks**." arXiv preprint arXiv:1603.01768 (2016). [Semantic Style Transfer](https://arxiv.org/abs/1603.01768)
5. Connelly Barnes, Eli Shechtman, Adam Finkelstein, and Dan B Goldman.
**PatchMatch: A Randomized Correspondence Algorithm for Structural Image Editing**.
ACM Transactions on Graphics (Proc. SIGGRAPH) 28(3), August 2009. [PatchMatch](https://gfx.cs.princeton.edu/pubs/Barnes_2009_PAR/index.php)
6. The codes in "image analogies" folder is built based on [neural image analogies](https://github.com/awentzonline/image-analogies) by Adam Wentz.

## Some Results

### Task #1: Painterly Rendering 3D Models (Non-photorealistic Rendering)

![image](https://github.com/jia-yi-chen/Illumination-guided-Neural-Style-Transfer/blob/master/figures/2.jpg)

### Task #2: Lanscape Painting

* robust to input photos containing a lot of sunlight (e.g., drawing sky)

![image](https://github.com/jia-yi-chen/Illumination-guided-Neural-Style-Transfer/blob/master/figures/1.jpg)
