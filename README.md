# PSTAN
PSTAN:A JND-aware Pairwise Spatio-Temporal Alignment Network for Compressed Videos Quality Enhancement.

# Requirements
Python>=3.7 Pytorch==1.3 NVIDIA GPU + CUDA
* Environment
```
conda create -n pstan python=3.7 -y && conda activate patan
git clone https://github.com/leryong/PSTAN
unzip PSTAN.zip && cd pstan
```
# Citation
If you use this code of our paper please cite:

```yaml
@article{yuan2026pstan,
  title={PSTAN: A JND-aware Pairwise Spatio-Temporal Alignment Network for Compressed Videos Quality Enhancement},
  author={Yuan, Yuan and Li, Eryong and Zhang, Jiawei and Ren, Jinchang and Lu, Xu},
  journal={IEEE Transactions on Circuits and Systems for Video Technology},
  year={2026},
  publisher={IEEE}
}
```


# Acknowledgments
This repository is implemented based on [BasicSR](https://github.com/XPixelGroup/BasicSR) and [VSR-Transformer](https://github.com/caojiezhang/VSR-Transformer). If you use the repository, please consider citing BasicSR,VSR-Transformer.
