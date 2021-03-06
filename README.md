# Project 4 Generative Visual

Lihang Gong, lgong@ucsd.edu

## Abstract

As a manga reader, I would be more delight to read colorized ones than gray-scaled ones. However, it takes much more additional efforts for manga creators to colorize. What if we have an auto painter that convert b&w manga into colorized ones? In this project, I developed a manga colorization solution based on pix2pix model. It is capabale of colorizing b&w manga pages based on some colorized samples. The future direction is to correct some inaccurate results and make them more natural.


## Model/Data

- Takes ~10 min to train the model.
- Training data is included in datasets/onepiece/A/.

## Code

- manga_colorization.ipynb: run this to simply regenerate the demonstrated results.  

For various usage:
- train.py: 
```
python train.py --dataroot path/to/datasets --name GIVE_A_NAME --model pix2pix --direction BtoA
```
- test.py:
```
python test.py --dataroot same/path/as/above --name SAME_NAME_AS_ABOVE --model pix2pix --direction BtoA
```

## Technical Notes

- Tested on Datahub.

## Reference

- [pix2pix paper](https://arxiv.org/pdf/1611.07004.pdf)
- [Pytorch implementation of pix2pix](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)

