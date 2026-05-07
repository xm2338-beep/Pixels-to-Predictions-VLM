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
