# PSTAN
PSTAN:A JND-aware Pairwise Spatio-Temporal Alignment Network for Compressed Videos Quality Enhancement.

# Requirements
Python>=3.7 Pytorch==1.3 NVIDIA GPU + CUDA
* Environment
```
conda create -n pstan python=3.7 -y && conda activate patan
git clone https://github.com/leryong/PSTAN
unzip PSTAN.zip && cd PSTAN

# given CUDA 11.6
python -m pip install torch==1.13.1+cu116 torchvision==0.14.1+cu116 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu116
python -m pip install tqdm lmdb pyyaml opencv-python scikit-image

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
