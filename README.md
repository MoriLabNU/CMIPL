# CMILP
A description projection for our Cross Margin-Information-based Pseudo-Label

# Data Preprocess

To prepare the dataset, you can follow the work of [WLSMIS](https://github.com/HiLab-git/WSL4MIS)

You can also run ```python code/scribbles_generator.py``` for scribble label generating and
```python code/dataloaders/word_data_processing.py``` for data preprocessing.

Our work is based on the 3D medical volumes.

The splits are available at ```./data/WORD```.



# Model Training
Run
```
CUDA_VISIBLE_DEVICES=0 python train_ours_refine.py --fold fold1 --seed 114514 --base_lr 3e-2 --num_classes 15 --batch_size 8 --exp WORD/s4mc_ours_crosspse
```
for model training.
Have fun.
