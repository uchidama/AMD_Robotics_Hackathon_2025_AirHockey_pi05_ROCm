# AMD_Robotics_Hackathon_2025_AirHockey_pi05_ROCm

![Mission 2 Air Hockey](mission2/video/mission2_airhockey.gif)

![npaka studio x EmplifAI Team Image](img/team_img.jpeg)

**Title:** AMD_RoboticHackathon2025-AirHockey_pi05_ROCm

**Team:** Team15: npaka studio x EmplifAI
* Hidekazu Furukawa
* Hiroyuki Osone
* Masatoshi Uchida

**Summary**
This project aims to enable the SO-101 robot arm to play Air Hockey. We utilized `lerobot` v0.4.1 for both data collection and inference processes. The model training was conducted on an AMD ROCm Cloud environment, specifically fine-tuning the pi0 (pi0.5) model. As a result, we successfully demonstrated the SO-101 performing Air Hockey tasks autonomously.


**How To**
1. **Data Collection**
   Create a dataset by playing Air Hockey. We used `lerobot` v0.4.1 for data collection.
2. **Training**
   Train the model on the AMD Dev Cloud environment using ROCm. We fine-tuned the `pi0` (pi0.5) model.
3. **Inference**
   Perform inference with the trained model using `lerobot` to control the robot arm.

**Delivery URL**

**Mission 1:**
![Mission 1 Picking](mission1/video/mission1_picking.gif)
- Dataset: [npaka/picking-amd-50](https://huggingface.co/datasets/npaka/picking-amd-50)
- Model: [npaka/picking-amd-50-pi05-50000](https://huggingface.co/npaka/picking-amd-50-pi05-50000)

**Mission 2:**
![Mission 2 Air Hockey](mission2/video/mission2_airhockey.gif)
- Dataset: [npaka/air-hockey-amd](https://huggingface.co/datasets/npaka/air-hockey-amd)
- Model: [npaka/air-hockey-amd-pi05-100000](https://huggingface.co/npaka/air-hockey-amd-pi05-100000)

**Directory Tree of this repo**

```terminal
AMD_Robotics_Hackathon_2025_AirHockey_pi05_ROCm/
├── README.md
├── Template-README.md
├── img
│   └── team_img.jpeg
├── mission1
│   ├── code
│   │   └── training-models-on-rocm-picking.ipynb
│   └── wandb
│       └── run-20251205_163409-t39l0540
└── mission2
    ├── code
    │   └── training-models-on-rocm-air-hockey.ipynb
    └── wandb
        ├── run-20251206_052705-s13hwsme
        └── run-20251206_091535-s13hwsme
```