# Deep-learning-based-resume-parser-and-analyzer
It is resume parser and analyzer based on Deep learning.
It automates the process of resume filtering.
It extracts and analyzes all important factor of resume like experience, education, project etc.

# How to use it

* A training data generation and annotation tool is created in the [scripts](scripts) folder which allows 
resume deep learning training data to be generated from any pdf and docx files stored in the 
[scripts/data/resume_samples](scripts/data/resume_samples) folder, To launch this tool, run the following 
command from the root directory of the project:

```batch
cd demo
python create_training_data.py
``` 

* After the training data is generated and annotated, one can train the resume parser by running the following
command:

```bash
cd demo
python dl_based_parser_train.py
```

* After the trained models are saved in the [scripts/models](scripts/models) folder,
one can use the resume parser to parse the resumes in the [scripts/data/resume_samples](scripts/data/resume_samples)
by running the following command:

```bash
cd demo
python dl_based_parser_predict.py
```

# Instructions
* You can train it on your own data.
* At present it only works on .pdf and .docx format.
* Motivation : chen0040

# Requirements
* Python 3.4+
* Tensorflow CPU/GPU
* Keras
* All basic Libraries : Numpy,Scipy,Matplotlib.

