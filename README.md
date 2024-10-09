# Curiosity-CEM
Official implementation of paper:

[Sample-efficient Real-time Planning with Curiosity Cross-Entropy Method and Contrastive Learning](https://arxiv.org/abs/2303.03787)

# Method
We propose Curiosity Cross-Entropy Method **(CCEM)**, an improved version of CEM for encouraging exploration via curiosity. CCEM optimizes trajectories by maximizing a discounted sum of Q values over the planning horizon. These Q values are trained to estimate future extrinsic and intrinsic rewards, hence encouraging reaching novel states. An _intrinsic curiosity module (ICM)_ is used to compute the intrinsic reward as the prediction error of the next latent state. We evaluate CCEM with [TD-MPC](https://github.com/nicklashansen/tdmpc), a capable model-based RL (MBRL) algorithm, and we utilize contrastive learning for efficient representation learning. **TD-MPC with CCEM** ouperforms previous MBRL algorithms in terms of _sample-efficiency_ and compares favorably with the best model-free algorithms on image-based control tasks from the [DeepMind Control Suite](https://github.com/deepmind/dm_control).


# Citation
cite the paper as follows:
```
@inproceedings{kotb2023sample,
  title={Sample-efficient real-time planning with curiosity cross-entropy method and contrastive learning},
  author={Kotb, Mostafa and Weber, Cornelius and Wermter, Stefan},
  booktitle={2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  pages={9456--9463},
  year={2023},
  organization={IEEE}
}
```
