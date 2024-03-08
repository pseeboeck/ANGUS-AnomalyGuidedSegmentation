# Anomaly guided segmentation: Introducing semantic context for lesion segmentation in retinal OCT using weak context supervision from anomaly detection

This is the github repository for the **anomaly guided segmentation (ANGUS)** approach. First anomaly-maps are created with a separate anomaly-detection model. Second, these binary anomaly-maps are added as an extra class for training the segmentation model. This provides additional semantic context without requiring extra manual labels. 
The work was accepted at the Medical Image Analysis Journal: [Paper](https://www.sciencedirect.com/science/article/pii/S136184152400029X) [^3]

[^3]: Seeböck, P., Orlando, J. I., Michl, M., Mai, J., Erfurth, U. S., & Bogunović, H. "Anomaly guided segmentation: Introducing semantic context for lesion segmentation in retinal OCT using weak context supervision from anomaly detection". Medical Image Analysis. 2024.


## Content

This repository contains 
 1. **anomaly maps** for the [RETOUCH challenge dataset](https://retouch.grand-challenge.org/) [^1] created by [WeakAND](https://ieeexplore.ieee.org/abstract/document/8727461) [^2] which were used as training targets for the ANGUS approach. --> folder 'RETOUCH Anomaly Maps'.
 2. **15 prediction maps** for the [RETOUCH challenge dataset - testset](https://retouch.grand-challenge.org/) [^1], created by  15 different models. 5 backbones (ANGUS-Net, ANGUS-Net-6,ANGUS-DeepLabv3, ANGUS-AttUNet, ANGUS-TransUNet) were trained for 3 different segmentation targets (IRC+Anomaly, SRF+Anomaly, PED+Anomaly) each (5*3=15). See also Table 1 and Table 2 of our paper. --> folder 'RETOUCH Prediction Maps'.
 3. **list of excluded Kermany-dataset samples**. We used the [Kermany-OCT2017 dataset](https://data.mendeley.com/datasets/rscbjbr9sj/2)[^4] in our experiments, with manual annotations from [here](https://vault.sfu.ca/index.php/s/0JwlgZ4IwRhmBkI?path=%2FFINAL_ATTEMPT%2FSegmentation)[^5]. As mentioned in the paper, we excluded 24 (DME) and 13 (DRUSEN) samples with invalid manual lesion annotations (e.g. non-closed contours) or other problems from our evaluation. --> folder 'KERMANY infos'.

[^1]: https://retouch.grand-challenge.org/
[^2]: Seeböck, Philipp, et al. "Exploiting epistemic uncertainty of anatomy segmentation for anomaly detection in retinal OCT." IEEE transactions on medical imaging 39.1 (2019): 87-98.
[^4]: https://data.mendeley.com/datasets/rscbjbr9sj/2
[^5]: https://vault.sfu.ca/index.php/s/0JwlgZ4IwRhmBkI?path=%2FFINAL_ATTEMPT%2FSegmentation, https://www.sciencedirect.com/science/article/pii/S1361841519300167

## Citation

*Seeböck, P., Orlando, J. I., Michl, M., Mai, J., Erfurth, U. S., & Bogunović, H. "Anomaly guided segmentation: Introducing semantic context for lesion segmentation in retinal OCT using weak context supervision from anomaly detection". Medical Image Analysis. 2024.*

```
@article{seebock2024anomaly,
  title={Anomaly guided segmentation: Introducing semantic context for lesion segmentation in retinal OCT using weak context supervision from anomaly detection},
  author={Seeb{\"o}ck, Philipp and Orlando, Jos{\'e} Ignacio and Michl, Martin and Mai, Julia and Erfurth, Ursula Schmidt and Bogunovi{\'c}, Hrvoje},
  journal={Medical Image Analysis},
  pages={103104},
  year={2024},
  publisher={Elsevier}
}
```
