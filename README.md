# GCRANet: Global Context Guided Refinement and Aggregation Network for Lightweight Surface Defect Detection

This official repository contains the source code of GCRANet. (accepted by PR2025).

Surface defect detection (SDD) is an important task in industrial manufacturing to ensure product quality, which is challenging due to weak defect appearances and background distractions. Despite the great advances in this task, few pixel-level defect detection methods achieve a satisfactory trade-off between accuracy and running efficiency. To this end, we develop a Global Context Guided Refinement and Aggregation Network (GCRANet) for lightweight surface defect detection, which fully utilizes global guidance to highlight defect details and suppress background noise in the lightweight network. Specifically, a lightweight Depthwise Self-Attention (DSA) module with linear complexity is introduced to capture global information based on deep features. Global information is combined with local features to capture more complete contours for weak defects. Furthermore, a Channel Cross-Attention (CCA) module is introduced to suppress background noise from multi-level features by exploiting channel dependencies between low-level features and semantic features. The experimental results on public defect datasets demonstrate that the proposed network achieves a better trade-off between accuracy and running efficiency than other state-of-the-art methods. Specifically, the proposed method achieves detection speed of 272.2 fps with 1.84M parameters, while yielding competitive accuracy (SD-saliency-900: WF of 91.79 %; Magnetic tile: WF of 80.64 %; DAGM 2007: WF of 86.53 %; CrackSeg9k: WF of 68.81 %; MVTec AD: WF of 80.37 % and 76.36 % on texture and object categories).


<img width="1706" height="748" alt="8f446d2a-b08b-4d22-a4ef-756539c4d286" src="https://github.com/user-attachments/assets/d798823e-a996-43d5-a45b-84c0e1322b69" />


## Data preparation

The training and test dataset can be downloaded at [google drive](https://drive.google.com/file/d/1DU32qPBn5hf35WOLI7XdoC5SdodwBJa-/view?usp=sharing)

## Results
We provide the predicted saliency maps at [google drive](https://drive.google.com/file/d/1-sKGHWghPuFUFJRXu0jzjeKYc6JDSHqd/view?usp=sharing)

## Citation
If you find our work useful in your research, please consider citing:
```
@article{yan2025global,
  title={Global Context Guided Refinement and Aggregation Network for Lightweight Surface Defect Detection},
  author={Yan, Feng and Jiang, Xiaoheng and Lu, Yang and Cui, Lisha and Cao, Jiale and Xu, Mingliang},
  journal={Pattern Recognition},
  pages={112893},
  year={2025},
  publisher={Elsevier}
}
```

