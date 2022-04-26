# CAS-771-project Classification with Noisy Labels

Before training the network:
!pip install chainer

!pip install chainercv

Put the noisy label files in the same directory as the python files.

To train the network in colab:

!python first_step_train.py --gpu 0 --out task1_1 --learnrate 0.08 --alpha 1.2 --beta 0.8

!python second_step_train.py --gpu 0 --out task1_2 --label task1_1
