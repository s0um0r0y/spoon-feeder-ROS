# Adaptive Robotic Manipulator Simulation for Enhanced Feeding and Drinking Assistance
Implemented reinforcement learning algorithms (PPO, SAC and DDPG) across different manipulators simulating feeding and drinking tasks on OpenAI gym, which was published in IEEE INDICON-24
conference [link of the paper](https://drive.google.com/file/d/1vM2wq5vHwwYHQxqxi9v7Wim37j7av-RD/view)

![image](https://github.com/user-attachments/assets/ac1ad11f-25f4-4e08-972a-c1c1983a688a)

## Getting Started

### Dependencies
* Pytorch
* OpenAI gym
* CUDA
* Ubuntu 20.04

### Installing
```bash
python3 -m pip install --upgrade pip
git clone https://github.com/s0um0r0y/spoon-feeder-ROS.git
cd spoon-feeder-ROS
python3 -m pip install -e .
```

### Train a new control policy
* running training (PPO)
  ```bash
  python3 -m assistive_gym.learn --env "ScratchItchJaco-v1" --algo ppo --train --train-timesteps 20000 --save-dir ./trained_models_new/
  ```
* visualizing the trained model
  ```bash
  python3 -m assistive_gym.learn --env "ScratchItchJaco-v1" --algo ppo --render --seed 0 --load-policy-path ./trained_models_new/
  ```

## Authors
Contributors names and contact info
- Soumo Roy [email id](soumoroy09@gmail.com)
- Joel Viju [email id](joelviju.v2021@vitstudent.ac.in)
- Budhaditya Bhattacharyya [email id](budhaditya@vit.ac.in)

## Video link
- [youtube link](https://youtu.be/lUmjaiPeUig?si=6kwH3TB_CEuhUNlX)
- [google drive link](https://drive.google.com/drive/folders/1jhOQWtvApqJR4CDxilfgPWyVUXPcWEZl?usp=sharing)

## Citations 
- Please consider citing us if you liked our project
```
@article{roy2025adaptiveroboticmanipulatorsimulation,
    title={Adaptive Robotic Manipulator Simulation for Enhanced Feeding and Drinking Assistance}, 
    author={Soumo Roy, Joel Viju and Budhaditya Bhattacharyya},
    year={2025},
    journal={IEEE India Council International Conference (INDICON)}
    url={https://doi.org/10.1109/INDICON63790.2024.10958301}, 
}
```
## License

This project is licensed under the [MIT] License - see the LICENSE.md file for details

## Acknowledgments
- I utilized [assistive gym](https://github.com/Healthcare-Robotics/assistive-gym) platform made by Dr. Zackory Erickson at CMU
- I would like to thank our professor [Dr. Budhaditya Bhattacharya](budhaditya@vit.ac.in) for his support, guidance and valuable time.
- This work was financialy supported by Vellore Institute of Technology (VIT), Vellore under the Faculty Seed Grant (RGEMS) (Sanction Order No.: SG20220001)
