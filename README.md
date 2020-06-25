# MCS Evaluation2 Submission: Usage README

## Download

Here are the instructions for downloading and setting up environment for MCS evaluation 2.

### Python Library

The latest release of the MCS Python library is `0.0.10`

1. Install the required third-party Python libraries:

```
pip install -r requirements.txt
```

2. Ensure you've installed `ai2thor` version `2.2.0`:

```
pip show ai2thor
```

3. Install the MCS Python Library:

```
pip install git+https://github.com/NextCenturyCorporation/MCS@latest
```

### Unity Application

The latest release of the MCS Unity app is `0.0.10`

1. [Download the Latest MCS Unity App](https://github.com/NextCenturyCorporation/MCS/releases/download/0.0.10/MCS-AI2-THOR-Unity-App-v0.0.10.x86_64)

2. [Download the Latest MCS Unity Data Directory TAR](https://github.com/NextCenturyCorporation/MCS/releases/download/0.0.10/MCS-AI2-THOR-Unity-App-v0.0.10_Data.tar.gz)

3. Ensure that both the Unity App and the TAR are in the same directory called "unity_app".

4. Untar the Data Directory:

```
tar -xzvf MCS-AI2-THOR-Unity-App-v0.0.10_Data.tar.gz
```

5. Mark the Unity App as executable:

```
chmod a+x MCS-AI2-THOR-Unity-App-v0.0.10.x86_64
```

5. Interaction tasks need a Metric-ff planer to run. This repo contains Mac version of it. You can goto the following website for the source code and compile it for your own system.

(https://fai.cs.uni-saarland.de/hoffmann/ff.html)

### Training Dataset

Interactive:
https://evaluation2-training-scenes.s3.amazonaws.com/interaction-scenes.zip

Intphys:
https://evaluation2-training-scenes.s3.amazonaws.com/intphys-scenes.zip


## Run with Interaction Task

```
python simple_task.py
```

## Run with Intuitive Physics Task

```
python int_phy_explain.py
```