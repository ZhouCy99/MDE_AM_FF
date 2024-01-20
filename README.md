# MDE_AM_FF

## Monocular Depth Estimation Based on Attention Mechanism and Feature Fusion Using Swin Transformer
This is the official PyTorch implementation for this paper. We will upload the complete code after the paper is accepted.

### Environment
python=3.8  pytorch=1.10.0  cudatoolkit=11.1

### Datasets
We used the datasets KITTI and NYU V2 for experiments and achieved certain results. If you want, You can prepare the datasets KITTI and NYUv2 according to [here](https://github.com/cleinc/bts), and then modify the data path in the config files to your dataset locations.


### Training
We use Swin Transformer as the Encoser, so you can download the pretrained bacbone from [here](https://github.com/microsoft/Swin-Transformer), and then modify the pretrain path .

Training the NYUv2 model:
```
python monoformer/train.py configs/arguments_train_nyu.txt
```

Training the KITTI model:
```
python monoformer/train.py configs/arguments_train_kittieigen.txt
```


### Evaluation
Evaluate the NYUv2 model:
```
python monoformer/eval.py configs/arguments_eval_nyu.txt
```

Evaluate the KITTI model:
```
python monoformer/eval.py configs/arguments_eval_kittieigen.txt
```

## Pretrained Models
To be updated...

## Citation
To be updated...

## Contact
For questions about our paper or code, please contact [us](https://github.com/ZhouCy99) or raise an issue on GitHub.



### Acknowledgements
Thanks to Microsoft Research Asia for opening source of the excellent work [Swin Transformer](https://github.com/microsoft/Swin-Transformer).
We repare the datasets according to [here](https://github.com/cleinc/bts).   We thank  Jin Han Lee for releasing the source code and the inspiring paper[BTS](https://arxiv.org/abs/1907.10326v5)


