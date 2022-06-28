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
# Current Setup

<i>Dataset:</i> CIFAR-10

<i>Model:</i> ResNet-18

The default parameters are provided in ```config.yaml```. One can vary the parameters by running ```python config_create.py```

In order to obtain selected checkpoints followed by data valuation and training the subset of data, run

```python experiment.py```

# Code Structure

The different modules in which this code repository has been organised is:

1. Dataset (dataset.py) - One can set up their own dataset as needed.

2. Model (model.py) - Different models can be added here.

3. Trajectory selection during training (run.py) - Selects checkpoints/trajectories along with training.

4. Value function definition and CheckSel algorithm (helper.py) - Different other value functions can be incorporated here.

5. Data valuation (scoreval_checksel.py) - Assigns scores to training datapoints using selected checkpoints/trajectories.

6. Subset selection (topsel.py or diverselect.py) - Returns a subset of datapoints as (a) top k elements or by (b) executing SimSel algorithm using the assigned scores. 
