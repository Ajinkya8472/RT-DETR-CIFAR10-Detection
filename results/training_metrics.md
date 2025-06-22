# RT-DETR Training Metrics

## Final Performance Results

| Metric | Value | Description |
|--------|-------|-------------|
| mAP@0.5-0.95 | 69.6% | Mean Average Precision across IoU thresholds 0.5-0.95 |
| mAP@0.5 | 72.6% | Mean Average Precision at IoU threshold 0.5 |
| mAP@0.75 | 72.6% | Mean Average Precision at IoU threshold 0.75 |
| Average Recall | 97.4% | Percentage of objects correctly detected |
| Training Time | ~50 minutes | Total time on Google Colab T4 GPU |
| Inference Speed | ~17 FPS | Frames per second during evaluation |

## Training Progress by Epoch

| Epoch | mAP@0.5-0.95 | mAP@0.5 | Loss | Learning Rate |
|-------|--------------|---------|------|---------------|
| 1 | 0.0% | 0.0% | 84.79 | 0.00001 |
| 2 | 11.2% | 18.3% | 45.16 | 0.00003 |
| 6 | 51.4% | 54.6% | 24.20 | 0.0001 |
| 11 | 69.6% | 72.6% | 22.27 | 0.0001 |

## Key Achievements

✅ Successfully converted CIFAR-10 classification to object detection format
✅ Achieved professional-grade mAP performance (69.6%)
✅ Maintained high recall (97.4%) - model finds almost all objects
✅ Optimized for Google Colab T4 GPU constraints
✅ Implemented complete MLOps pipeline with automated backups

## Technical Configuration

- **Model**: RT-DETR with ResNet-50 backbone
- **Dataset**: 800 training images, 200 validation images
- **Image Size**: 128x128 pixels (upscaled from CIFAR-10's 32x32)
- **Batch Size**: 4 (optimized for T4 GPU memory)
- **Epochs**: 12 total epochs
- **Best Model**: Saved at epoch 11
