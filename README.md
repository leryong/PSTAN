# PSTAN
PSTAN:A JND-aware Pairwise Spatio-Temporal Alignment Network for Compressed Videos Quality Enhancement.

# Requirements
Python>=3.7 Pytorch>=1.1 NVIDIA GPU + CUDA
* Environment
```
conda create -n pstan python=3.7 -y && conda activate pstan
git clone https://github.com/leryong/PSTAN
unzip PSTAN.zip && cd PSTAN

# given CUDA 11.6
pip install torch==1.13.1+cu116 torchvision==0.14.1+cu116 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu116
pip install -r requirements.txt
```

* DCNv2  
```
cd ops/dcn/  
bash build.sh
```
* VideoSet dataset  
You can get the dataset from [VideoSet](http://ieee-dataport.org/documents/videoset).

# Train
```
python basicsr/train.py --opt_path ./options/train/train_videoset.yaml
```

# Test
```
python basicsr/test.py --opt_path ./options/test/test_PSTAN_videoset.yaml
```


# Citation
If you use this code of our paper please cite:

```yaml
@ARTICLE{11367012,
  author={Yuan, Yuan and Li, Eryong and Zhang, Jiawei and Ren, Jinchang and Lu, Xu},
  journal={IEEE Transactions on Circuits and Systems for Video Technology}, 
  title={PSTAN: A JND-Aware Pairwise Spatio-Temporal Alignment Network for Compressed Videos Quality Enhancement}, 
  year={2026},
  volume={36},
  number={6},
  pages={8491-8505},
  keywords={Videos;Training;Image coding;Visualization;Quality assessment;Optical flow;Circuits and systems;Transformers;Motion compensation;Image restoration;Compressed video quality enhancement (CVQE);pairwise spatio-temporal alignment network (PSTAN);just noticeable difference (JND)},
  doi={10.1109/TCSVT.2026.3658352}}
```

# Acknowledgments
This repository is implemented based on [BasicSR](https://github.com/XPixelGroup/BasicSR) and [VSR-Transformer](https://github.com/caojiezhang/VSR-Transformer). If you use the repository, please consider citing BasicSR,VSR-Transformer. Also, thanks to [VideoSet](http://ieee-dataport.org/documents/videoset) for providing the dataset.
