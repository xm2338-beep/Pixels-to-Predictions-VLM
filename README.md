# Pixels-to-Predictions-VLM
Fine-tuning SmolVLM-500M-Instruct with LoRA/DoRA for scientific visual multiple-choice reasoning on the ScienceQA Kaggle competition.

### Repository Contents
Pixels-to-Predictions-VLM.ipynb : Main notebook for training and inference  
requirements.txt : Required Python packages  

### Model Weights
The fine-tuned model adapter weights are hosted on Hugging Face:
https://huggingface.co/OwlCastle/SmolVLM-500M-ScienceQA-Model-Weights/tree/main

### Base Model
https://huggingface.co/HuggingFaceTB/SmolVLM-500M-Instruct

### Training Features
LoRA + DoRA fine-tuning  
PEFT-based training pipeline  
448×448 image processing    
Gradient accumulation  
Gradient checkpointing  
Visual data augmentation  
Structured prompt engineering  

### Notes
The notebook contains the complete training and inference pipeline  
The repository was developed for offline Kaggle evaluation  
The Hugging Face repository contains the exported adapter weights and tokenizer files  

### Requirements
Main dependencies:  

transformers  
peft  
torch  
bitsandbytes  
accelerate  
datasets  
pillow  

See requirements.txt for details.  

### proper reproducable steps

The results can be fully reproduced by directly running the provided notebook in the original Kaggle competition environment. For reproduction in Google Colab or other local environments, users may need to modify the dataset loading paths to match their own directory structure. For fully offline reproduction without internet access, locate the cell titled “Local offline model loading version” in the notebook, uncomment the following two lines:  
  
LOCAL_MODEL_PATH = "your path"  
MODEL_ID = LOCAL_MODEL_PATH  
  
and replace "your path" with the local path to the downloaded base model. The base model download link is provided above in the README.  






