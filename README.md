# BrainTumorDetection
Detecting brain tumor and its type from MRI scans.
Originally dataset was taken from here:
https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri
After combing two more datasets i noticied that model performance did not seem to get better as some pictures were incorrrectly labelled in the original dataset.
Fortunately, i found another dataset on kaggle which worked. The dataset currently used is:
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset?select=Training
I created two models, the first model is relatively simple and the second is more complex. Feel free to experiment with both models although the first (the simpler) model does better than the one that is complex.
Overall evaluation on the test set is as follows:

Tumor vs Non Tumor class:

![heatmap_1](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/48979d04-8c29-4bcd-bfdd-92dec77a5a06)
![heatmap_2](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/ca75c2a8-b9ff-4446-ae13-00347a849a8f)

Tumor and its types:

![heatmap_3](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/bebc4c2a-f7bf-4731-8f80-4047e8afd337)
![heatmap_4](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/d82ce2fa-96d1-4475-b87d-c7b240fb7149)

Losses and Accuracy curves:

![losses curve](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/d7a7396d-9e2e-4e7e-836a-d9d9aa0e329e)
![accuracy curve](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/d2a88089-dfb5-4608-bfe9-ae361d973734)


Model Architecture:

![model](https://github.com/rajasarmadishtiaq/BrainTumorDetection/assets/60262105/32a9f9ec-cbca-4c6c-93eb-6d3426ba6284)

Additional image preprocessing can be done and i am confident it *might* improve the model. Furthermore, an interesting thing to research would be to balance the total images for tumor classes i.e., meningioma + glioma + pituitary and non tumor class by increasing the amount of images in the non tumor class. The model perfomance *might* also increase with this addition.
