# CheckSel

<i>Paper:</i> [CheckSel: Efficient and Accurate Data-valuation Through Online Checkpoint Selection](https://arxiv.org/abs/2203.06814)
<i>Authors:</i> Soumi Das, Manasvi Sagarkar, Suparna Bhattacharya, Sourangshu Bhattacharya

# Getting Started

Run the following commands to setup the environment:

```
git clone https://github.com/SoumiDas/CheckSelect.git

cd CheckSelect

pip install requirements.txt

```
# Execution

The default parameters are provided in ```config.yaml```. One can play around with the parameters by running ```python config_create.py```

In order to obtain selected checkpoints followed by data valuation and training the subset of data, run

```python experiment.py```

The current setup is for CIFAR-10 dataset and ResNet-18 model. However, one can change as per their requirements in ```dataset.py``` and ```model.py```
