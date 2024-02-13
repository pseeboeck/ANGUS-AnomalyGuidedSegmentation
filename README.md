# Anomaly guided segmentation: Introducing semantic context for lesion segmentation in retinal OCT using weak context supervision from anomaly detection

This is the github repository for the **anomaly guided segmentation (ANGUS)** approach. First anomaly-maps are created with a separate anomaly-detection model. Second, these binary anomaly-maps are added as an extra class for training the segmentation model. This provides additional semantic context without requiring extra manual labels. 
The work was accepted at the Medical Image Analysis Journal: [Paper](https://www.sciencedirect.com/science/article/pii/S136184152400029X)




## Content

This repository contains the **anomaly maps** for the [RETOUCH challenge dataset](https://retouch.grand-challenge.org/)[^1] created by [WeakAND](https://ieeexplore.ieee.org/abstract/document/8727461)[^2] which were used as training targets for the ANGUS approach.

[^1]: https://retouch.grand-challenge.org/
[^2]: Seeböck, Philipp, et al. "Exploiting epistemic uncertainty of anatomy segmentation for anomaly detection in retinal OCT." IEEE transactions on medical imaging 39.1 (2019): 87-98.


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
