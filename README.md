# MRC²VD: A Multimodal Remote Cardiac Cycle-Level Variability Dataset of Physiological Signals

## Overview

MRC²VD is a multimodal dataset of cardiac physiological signals. It includes synchronized recordings of electroencephalogram (EEG), electrocardiogram (ECG), photoplethysmogram (PPG), ballistocardiogram (BCG), chest pressure-based respiratory signals, blood oxygen saturation (SpO₂), and facial video data, from which remote photoplethysmography (rPPG) signals can be derived.

ECG, PPG, BCG, and video-derived rPPG serve as the **core modalities** for heart rate (HR) and heart rate variability (HRV) analysis, while EEG, respiratory, and SpO₂ signals are provided as **auxiliary modalities** to support exploratory research on cross-modal physiological coupling.

## Dataset

- **Science Data Bank record**: https://doi.org/10.57760/sciencedb.29362
- **CSTR**: https://cstr.cn/31253.11.sciencedb.29362
- **Version**: V4
- **Published**: 2025-10-14
- **Last updated**: 2026-09-10
- **Access**: Restricted access for facial video recordings; physiological signal data (CSV) are openly accessible.
- **License**: The dataset is governed by the Data Usage Agreement (DUA). See the DUA section below.

## Data Usage Agreement (DUA)

Access to the facial video recordings requires completion of the Data Usage Agreement (DUA), available at:

https://www.scidb.cn/static/dataSet/restrictedfile/694480ac65244451b1094d6d6dd7d980/V5/author/MRC2VD_Data_Usage_Agreement.pdf

Applicants are required to provide their full name, position, institutional affiliation, and a brief description of the intended use of the dataset. For a student applicant, please provide your supervisor's information and ask your supervisor to sign the agreement; the application email should copy the supervisor.

Access requests are typically processed within 5–7 business days.

## Code

This repository contains the source code for the investigations in the associated manuscript, including:

- rPPG extraction and benchmarking (GRGB, GREEN, CHROM, POS, ICA, PCA);
- heart rate estimation from ECG, PPG, BCG, and video-derived rPPG;
- HRV analysis (Mean RR, LF/HF) on Task 3;
- multimodal fusion with dynamic gating (illustrative case study).

The dataset itself is **not** hosted in this repository. Please obtain the data through Science Data Bank following the DUA process described above.

## Installation

```bash
git clone https://github.com/YuanwangWei2000/MRC2VD.git
cd MRC2VD
pip install -r requirements.txt
```

## Citation

If you use this dataset or code, please cite the dataset:

> Zhou Caiying, Zeng Luhang, Zhou Yuhao, Wei Yuanwang, Fried-Michael Dahlweid, Wang Sheng, Sun Hong, Wang Chaochao, Zhang Xianchao. Multimodal Remote Cardiac Cycle-Level Variability Dataset (MRC²VD)[DS/OL]. V4. Science Data Bank, 2026. https://doi.org/10.57760/sciencedb.29362.

>@misc{dataset_mrc2vd,
  author       = {Zhou, Caiying and Zeng, Luhang and Zhou, Yuhao and Wei, Yuanwang and
                  Dahlweid, Fried-Michael and Wang, Sheng and Sun, Hong and
                  Wang, Chaochao and Zhang, Xianchao},
  title        = {Multimodal Remote Cardiac Cycle-Level Variability Dataset ({MRC}$^2${VD})},
  year         = {2026},
  version      = {V4},
  publisher    = {Science Data Bank},
  doi          = {10.57760/sciencedb.29362},
  url          = {https://doi.org/10.57760/sciencedb.29362},
  note         = {Dataset}
}
If the corresponding methodology paper is published, please also cite it in addition to the dataset.



## License

The **source code** in this repository is licensed under the **MIT License**. See the `LICENSE` file for details.

The **dataset** is hosted on Science Data Bank and is **not** covered by the MIT License. Its access and use are governed by the Data Usage Agreement (DUA):

https://www.scidb.cn/static/dataSet/restrictedfile/694480ac65244451b1094d6d6dd7d980/V5/author/MRC2VD_Data_Usage_Agreement.pdf

Please note that the DUA prohibits re-identification and redistribution of the facial video recordings.

## Contact

For questions about the dataset or access requests, please contact:

- yuanwang_wei@zjxu.edu.cn
