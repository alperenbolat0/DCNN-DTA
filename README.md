#  DCCN-DTA: deep drug-target binding affinity prediction

This document is  prepared as a project for the Bioinformatic course at TOBB ETU University.this project uses DeepDTA's datasets and subsystems. The motivation of the project is to suggest a more successful and efficient deep learning model.

By Alperen Bolat

 <img src="https://github.com/alperenbolat0/DCNN-DTA/blob/master/docs/figures/bioenformatic%20figure%202.png" width="400" height="800">
# Installation

## Data

Please see the [readme](https://github.com/hkmztrk/DeepDTA/blob/master/data/README.md) for detailed explanation.

## Requirements

You'll need to install following in order to run the codes.

*  [Python 3.4 <=](https://www.python.org/downloads/)
*  [Keras 2.x](https://pypi.org/project/Keras/)
*  [Tensorflow 1.x](https://www.tensorflow.org/install/)
*  numpy
*  matplotlib

You have to place "data" folder under "source" directory. 

# Running baseline
```

python run_baseline.py --num_windows 32 \
                          --seq_window_lengths 12 \
                          --smi_window_lengths 8 \
                          --batch_size 256 \
                          --num_epoch 100 \
                          --max_seq_len 1000 \
                          --max_smi_len 100 \
                          --dataset_path 'data/kiba/' \
                          --problem_type 1 \
                          --log_dir 'logs/'


```
# Running proposed model
```
python run_master.py --num_windows 32 \
                          --seq_window_lengths 12 \
                          --smi_window_lengths 8 \
                          --batch_size 256 \
                          --num_epoch 100 \
                          --max_seq_len 1000 \
                          --max_smi_len 100 \
                          --dataset_path 'data/kiba/' \
                          --problem_type 1 \
                          --log_dir 'logs/'


```





