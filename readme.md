
---

# Fine-Tuning BLIP Model on Flickr 8k Dataset Using PEFT LoRA

This repository contains the implementation and results of fine-tuning the BLIP (Bootstrapping Language-Image Pretraining) model on the Flickr 8k dataset using Parameter-Efficient Fine-Tuning (PEFT) with LoRA (Low-Rank Adaptation). The project aims to enhance the model's ability to generate descriptive captions for images.

## Project Overview

The BLIP model is a state-of-the-art architecture for image captioning and visual question answering. By fine-tuning the model on the Flickr 8k dataset, we leverage LoRA, a PEFT technique, to achieve efficient training and improve the model's performance in generating accurate and meaningful captions.

## Dataset

### Flickr 8k
The Flickr 8k dataset consists of 8,000 images, each paired with five different captions. The dataset is widely used for training and evaluating image captioning models.

## Approach

### Preprocessing
- **Image Preprocessing**: Images are resized and normalized to match the input requirements of the BLIP model.
- **Text Preprocessing**: Captions are tokenized and converted into a format suitable for training.

### Fine-Tuning
- **Base Model**: BLIP (Bootstrapping Language-Image Pretraining).
- **Technique**: PEFT LoRA (Low-Rank Adaptation).
- **Optimizer**: AdamW with a learning rate of 5e-5.
- **Training Details**: The model is trained for 10 epochs with early stopping based on validation loss.

## Results

### Evaluation Methodology
The model was evaluated by generating captions for images in the validation dataset and comparing them with the ground truth captions.

## Conclusion

The fine-tuning of the BLIP model using PEFT LoRA on the Flickr 8k dataset has shown significant improvements in the model's ability to generate accurate and descriptive captions for images. This approach demonstrates the effectiveness of using PEFT techniques for efficient and scalable model training.

---
