# YOLOv7 Safety Use Case Tutorial

This repository contains a Jupyter Notebook that must be run alongside the **SageMaker Image** available at [developer.sima.ai](https://developer.sima.ai). The notebook walks through the following steps:

1. **Retraining YOLOv7** on a safety-related dataset.
2. **Exporting** the trained model to ONNX.
3. **Performing "Surgery"** on the ONNX model (graph manipulation).
4. **Quantizing** the model.
5. **Compiling** the model to create a binary for the Sima.ai MLSoC platform.
6. **Packaging and uploading** the resulting `.tar.gz` artifact to an S3 bucket.

## Prerequisites

- AWS account with permissions to use SageMaker.
- Access to the SageMaker Image from [developer.sima.ai](https://developer.sima.ai).
- An S3 bucket for uploading the final `.tar.gz`.

## Usage

1. **Launch SageMaker Notebook**:  
   - Select the Sima.ai image when creating a new SageMaker Notebook instance.
   
2. **Clone this repository** in your SageMaker environment:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
