# MedFusion: A Unified Vision-Language Framework for Radiology Images

## Overview

MedFusion is an AI-powered multimodal system for medical image analysis that combines advanced vision transformers with specialized language models to provide accurate diagnostic insights, medical report generation, and visual question answering for radiology images.

📹 **[View Demo Video](https://github.com/ThiruDeepak2311/MedRepImg/issues/1)**

## Key Features

- **Medical Visual Question Answering (VQA)** - Answer clinical questions about medical images
- **Automated Report Generation** - Generate comprehensive medical reports from radiology scans  
- **Disease Detection & Identification** - Identify pathologies and abnormalities
- **Multilingual Support** - English and Tamil language capabilities
- **Voice Interaction** - Hands-free operation with speech-to-text/text-to-speech
- **Multi-modal Input** - Supports X-rays, CT scans, MRIs, and ultrasound images

## Architecture

### Multi-Encoder Visual System
- **Pyramid V2 Transformer** - Overlapping patch processing for fine-grained detail extraction
- **ConvNeXt** - CNN-based encoder for structural pattern recognition  
- **CLIP (ViT-32B)** - Vision transformer for semantic understanding

### Language Model
- **Med-LLaMA** - LLaMA 3 fine-tuned on PubMedQA for medical domain expertise
- **Feature Concatenation Layer** - Deep alignment network for visual-textual integration

## Performance

| Dataset | Accuracy |
|---------|----------|
| SLAKE   | 76.3%    |
| PMC-VQA | 72.8%    |
| RadVQA  | 66.0%    |

*Represents 7.8% average improvement over previous state-of-the-art methods*

## Training Data

- **ROCO** - 81k+ radiology images with captions
- **MedICaT-200k** - Medical images with captions and tabular data
- **PMC VQA** - Medical visual question-answer pairs from PubMed Central
- **PubMedQA** - 273k biomedical question-answer pairs
- **SLAKE** - Bilingual medical VQA dataset

## Technical Highlights

- **R3 StyleGAN** data augmentation for medical image synthesis
- **InfoNCE contrastive learning** for vision-language alignment
- **Cross-modal attention** mechanism for visual-textual grounding
- **Multi-stage training pipeline** with frozen encoders and fine-tuned language model

## Interface

Web-based Gradio interface supporting:
- Image upload and analysis
- Text and voice queries
- Real-time translation (English ↔ Tamil)
- Medical report export
- Hands-free operation mode

## Installation & Usage

```bash
# Clone repository
git clone [repository-url]
cd MedFusion

# Install dependencies
pip install -r requirements.txt

# Run the application
python app.py
```

## Citation

```bibtex
@article{medfusion2025,
  title={MedFusion: A Unified Vision-Language Framework for Radiology Images},
  author={Akhshan P, Deepak T, Janani Harshatha J, Karthick N G},
  journal={Shiv Nadar University Chennai},
  year={2025}
}
```

## License

This project is developed as part of a Bachelor of Technology thesis in Artificial Intelligence & Data Science at Shiv Nadar University Chennai.

---

**Note**: This system is designed to assist medical professionals and should not replace clinical judgment or professional medical advice.
