# Artificial Intelligence: Course Assignments

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-F9AB00?logo=googlecolab&logoColor=white)

Assignments from the Artificial Intelligence course in my B.S. AI program at Kookmin University. Each notebook runs in Google Colab.

## Assignments

| # | Notebook | Topic | Result |
| --- | --- | --- | --- |
| 1 | [Perceptron](AI_Assignment1_20252403_%EC%9D%B4%EC%8A%AC%EB%A1%AC%EB%B2%A1.ipynb) | Perceptron with fully **vectorized** `evaluate` and `train` (no Python loops), decision boundary plotted before and after training | Linear classifier on a 2-D toy dataset |
| 2a | [MLP on CIFAR-10](AI_Assignment2_MLP_20252403_%EC%9D%B4%EC%8A%AC%EB%A1%AC%EB%B2%A1.ipynb) | 4-layer MLP (3072→1024→512→256→10) with BatchNorm, Dropout and Adam | **58.8%** test accuracy |
| 2b | [CNN on CIFAR-10](AI_Assignment2_CNN_20252403_%EC%9D%B4%EC%8A%AC%EB%A1%AC%EB%B2%A1_v2.ipynb) | 6-layer CNN (32→64→128 channels) with BatchNorm, Dropout, Adam, weight decay and a cosine LR schedule | **87.6%** test accuracy |

The two CIFAR-10 models were trained for 30 epochs each. They show how much the convolutional inductive bias helps on images: the CNN beats the MLP by about 29 percentage points.

## Run

Open any notebook and click the **Open in Colab** badge at the top. The CIFAR-10 notebooks download the dataset from Hugging Face (`uoft-cs/cifar10`), and a GPU runtime is recommended. The perceptron notebook expects `perceptron_toydata.txt` in the working directory.
