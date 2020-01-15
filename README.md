# Self Using Note

[![Badge](https://img.shields.io/badge/link-996.icu-%23FF4D5B.svg?style=flat-square)](https://996.icu/#/en_US)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg?style=flat-square)](https://github.com/996icu/996.ICU/blob/master/LICENSE)

**Some Useful Niubi** tricks, repositories and paper. Just use Ctrl+F and input key words to search what you what. ~~Strikethrough~~ means I have not gone through yet.

## General Structure
[Bilinear pooling](https://arxiv.org/pdf/1511.06062.pdf): Outer multiply two features. A sample code for bilinear pooling is [here] (https://github.com/yuminsuh/part_bilinear_reid/blob/21ea0906cb583312c382eb997b79913046c88a5b/reid/models/CompactBilinearPooling_dsybaik.py#L15) and [here](https://github.com/HaoMood/bilinear-cnn) and [here](https://github.com/Iceland-Leo/Bilinear-CNN/blob/master/bilinear_resnet.py).

~~[Bilinear pooling in application](http://vis-www.cs.umass.edu/bcnn/docs/bcnn_iccv15.pdf)~~

[High Resolution Net(HRNet)](https://arxiv.org/abs/1904.04514): UNet with convolution in skip connection.

[DANet](https://arxiv.org/abs/1809.02983): Dual self attention module, great example of [pytorch sync-batch-norm and attention module](https://github.com/junfu1115/DANet).

[XceptionNet](https://arxiv.org/abs/1610.02357): Reverse seperable convolution without activation.

~~[Independent Components Layer](https://arxiv.org/abs/1905.05928v1): Combination of batch normalization and dropout layer.~~

~~[Adaptive Batch Normalization](https://arxiv.org/abs/1603.04779): Related paper [AdaIN](https://arxiv.org/abs/1703.06868)~~

## Detection
[Uncertainty bounding box](https://arxiv.org/abs/1809.08545)

## Face Recognition
~~[Deep Comparator Network](https://arxiv.org/abs/1807.11440)~~

~~[SBR landmark detector](https://arxiv.org/abs/1807.00966): An Unsupervised Approach to Improve the Precision of Facial Landmark Detectors. [Github](https://github.com/D-X-Y/landmark-detection)~~

## Image Synthesis
[Few shot unsupervised image2image](https://arxiv.org/abs/1905.01723): Content module and style module.

[Pix2PixHD: Segmentation to image](https://arxiv.org/abs/1711.11585): Enhancer structure.

[Semantic Image Synthesis with Spatially-Adaptive Normalization(SPADE)](https://arxiv.org/abs/1903.07291): Used in GauGAN, segmentation to image.

[SinGAN](https://arxiv.org/abs/1905.01164): Using multiscale patch generator to learn the distribution of target nature image.(ICCV19 Best Paper)

[AdaIN](https://arxiv.org/abs/1703.06868): Adaptive instance normalization using in style transfer. Related paper [AdaBN](https://arxiv.org/abs/1603.04779)

~~[Domain Intersection and Domain Difference](https://arxiv.org/abs/1908.11628)~~

[styleGAN](https://arxiv.org/abs/1812.04948): Really impressive with interesting structure. Eight FCs as guidance. Repo is [here](https://github.com/NVlabs/stylegan).

[styleGAN2](http://arxiv.org/abs/1912.04958): Handle with naughty artifacts in styleGAN. Repo is [here](https://github.com/NVlabs/stylegan2).

### Face swapping: from beginner to give-up
[Face Swapping GAN(FSGAN)](https://arxiv.org/abs/1908.05932): Subject agnostic face swapping and reenactiment model.

[Face swapping GAN](https://github.com/shaoanlu/faceswap-GAN): Introducing self attention, Kalman Filter.

[Few-shot Realistic Neural Talking Head Models](https://arxiv.org/pdf/1905.08233.pdf): Few-shot talking face sequences generator as one of the baselines of face swapping.

[Few-shot face swapping GAN](https://github.com/shaoanlu/fewshot-face-translation-GAN): Introducing AdaIN, SPADE.

[Deep face lab](https://github.com/iperov/DeepFaceLab): ~~deep cyka blyat learning!~~ Deep fake tools.

[Expression transfer network](https://arxiv.org/pdf/1909.02967.pdf): Which is basically one of my original ideas and someone just realised it. Research is struggle.

### Deepfake Detection and related works
[DFDC dataset](https://deepfakedetectionchallenge.ai/)

[Celeb-DF dataset](https://arxiv.org/abs/1909.12962)

[FaceForensics++ dataset](https://github.com/ondyari/FaceForensics/)

[FaceForensics dataset](https://arxiv.org/abs/1803.09179)

[A deepfake detection repository](https://github.com/dessa-public/DeepFake-Detection)

[Face X-ray](https://arxiv.org/pdf/1912.13458.pdf): Detect forgery depending on blending patterns, SOTA approach of deepfake detection.

[DSP-FWA](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Li_Exposing_DeepFake_Videos_By_Detecting_Face_Warping_Artifacts_CVPRW_2019_paper.pdf): The improved version is available [here](https://github.com/danmohaha/DSP-FWA)

### Video general noise feature (PRNU) and steganalysis

[Get rich feature from SRM filter](https://arxiv.org/pdf/1805.04953.pdf): Inspired by [Rich Models steganalysis](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.441.6997&rep=rep1&type=pdf) to detect photoshop modification.

[Yedroudj-Net for steganalysis](https://arxiv.org/pdf/1803.00407.pdf)

[Sensor pattern noise identification](https://www.researchgate.net/publication/3455253_Digital_Camera_Identification_From_Sensor_Pattern_Noise)

[Color-Decoupled Photo Response Non-Uniformity](https://ieeexplore.ieee.org/document/5934587)

[BOSS dataset for steganalysis](https://hal.archives-ouvertes.fr/hal-00648057/document)

### rPPG or related biology pattern (Warning: 玄学)
[rPPG](http://openaccess.thecvf.com/content_ECCV_2018/papers/Siqi_Liu_Remote_Photoplethysmography_Correspondence_ECCV_2018_paper.pdf):  Recommended by ZK.W

[Another rPPG](https://ieeexplore.ieee.org/document/8575334/versions): Not really novel.

[A repo of rPPG](https://prouast.github.io/heartbeat-js/)

## 3D
[Active Appearance Model](https://www.cs.cmu.edu/~efros/courses/LBMV07/Papers/cootes-eccv-98.pdf)

[Thin Plate Spline Interpolation](https://en.wikipedia.org/wiki/Thin_plate_spline)

### 3D morphable model: from beginner to give-up
[Basel Model 09](https://gravis.dmi.unibas.ch/publications/2009/BFModel09.pdf): Standard face 3DMM.

[Basel Model 17](https://arxiv.org/abs/1709.08398): Standard face 3DMM. Optimize facial expression.

[Gaussian morphable model](https://arxiv.org/pdf/1603.07254v1.pdf): Introduction of Gaussian 3DMM.

~~[Markov Chain Monte Carlo for Automated Face Image Analysis](https://link.springer.com/article/10.1007%2Fs11263-016-0967-5)~~

[DF2Net](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zeng_DF2Net_A_Dense-Fine-Finer_Network_for_Detailed_3D_Face_Reconstruction_ICCV_2019_paper.pdf): Deep learning approach single image 3DMM generator.

[Deep 3D face reconstruction](https://arxiv.org/abs/1903.08527): Code available [here](https://github.com/microsoft/Deep3DFaceReconstruction)

[3D face alignment](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/main.htm): 3dmm data and code.

[Python 3dmm tools](https://github.com/YadiraF/face3d)

[Another deep 3D face reconstruction](https://arxiv.org/abs/1903.10873): Code available [here](https://github.com/apchenstu/Facial_Details_Synthesis)

## Video Generation
~~[MoCoGAN](http://openaccess.thecvf.com/content_cvpr_2018/papers/Tulyakov_MoCoGAN_Decomposing_Motion_CVPR_2018_paper.pdf): Video generation and enhancement~~

## Low Level Vision
~~[Deep Image Prior](https://arxiv.org/abs/1711.10925): VGG will have better result using in perceptual loss compared with ResNet.~~

## Loss Function
[Triple consistency loss for pairing distributions in GAN-based face synthesis](https://arxiv.org/abs/1811.03492): Combination of long path loss and short cut loss.

Give wrong labeled pixel penalty:
lossfunction(out,gt,reduction=None)*|Sig(out)-gt|

Hinge loss:
loss=max(0,1-gt*out)

## Explainability and Interpretability
~~[Explaining Explanations: An Overview of Interpretability of Machine Learning](https://arxiv.org/abs/1806.00069)~~

## Not classified yet

http://openaccess.thecvf.com/content_ECCV_2018/papers/Yaojie_Liu_Face_De-spoofing_ECCV_2018_paper.pdf
