# CMIPL
A description projection for our Cross Margin-Information-based Pseudo-Label

# Data Preprocess

To prepare the dataset, you can follow the work of [WLSMIS](https://github.com/HiLab-git/WSL4MIS)

You can also run ```python code/scribbles_generator.py``` for scribble label generating and

```python code/dataloaders/word_data_processing.py``` for data preprocessing.

Our work is based on 2D medical CT images.




# Model Training
Run
```
CUDA_VISIBLE_DEVICES=0 python train_ours_refine.py --fold fold1 --seed 114514 --base_lr 3e-2 --num_classes 15 --batch_size 8 --exp ours_cmipl
```
for model training.
Have fun.
