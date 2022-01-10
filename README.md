# Dubai-Satellite-Imagery-Multiclass-Segmentation

## Note: Use Jupyter NbViewer to load the code if GitHub doesn't render

Please copy the links of the .ipynb files and paste it in [NbViewer](https://nbviewer.org/) if GitHub fails to load it in the browser.

## Dataset
<p align="justify">
<a href="https://humansintheloop.org/">Humans in the Loop</a> has published an open access dataset annotated for a joint project with the <a href="https://www.mbrsc.ae/">Mohammed Bin Rashid Space Center</a> in Dubai, the UAE. The dataset consists of aerial imagery of Dubai obtained by MBRSC satellites and annotated with pixel-wise semantic segmentation in 6 classes. The images were segmented by the trainees of the Roia Foundation in Syria.
</p>

The images are densely labeled and contain the following 6 classes:

| Name       | R   | G   | B   | Color |
| ---------- | --- | --- | --- |-------|
| Building   | 60  | 16  | 152 |![#3b1098](https://via.placeholder.com/15/3b1098/000000?text=+) `#3b1098`|
| Land       | 132 | 41  | 246 |![#8529f6](https://via.placeholder.com/15/8529f6/000000?text=+) `#8529f6`|
| Road       | 110 | 193 | 228 |![#6ec1e4](https://via.placeholder.com/15/6ec1e4/000000?text=+) `#6ec1e4`|
| Vegetation | 254 | 221 | 58  |![#fedd3a](https://via.placeholder.com/15/fedd3a/000000?text=+) `#fedd3a`|
| Water      | 226 | 169 | 41  |![#e2aa29](https://via.placeholder.com/15/e2aa29/000000?text=+) `#e2aa29`|
| Unlabeled  | 155 | 155 | 155 |![#9b9b9b](https://via.placeholder.com/15/9b9b9b/000000?text=+) `#9b9b9b`|

## Benchmark Models
- [Standard U-Net](./01-01-Standard_U-Net.ipynb)
- [U-Net with Resnet Backbone](./01-02-Unet_with_Resnet_Backbone.ipynb)
- [DeepLabV3+](./01-03-DeepLabV3%2B_Model.ipynb)

## Transfer Learning from InceptionResNetV2 to U-Net CNN
- [Data Augmentation](./02-01-Dataset_Augmentation.ipynb)
- [Model Training and Evaluation](./02-02-Transfer_Learning_InceptionResNetV2_and_U-Net.ipynb)

## Software & Libraries
- Python >=3.*
- NumPy
- Pandas
- Matplotlib
- IPython
- Open-CV
- Tensorflow
- Keras
- Patchify
- Segmentation models
- Albumentations
