
# **Optimized U-Net Implementation for Brain Tumor Segmentation**

## **Description**

This project focuses on optimizing the U-Net architecture for 2D brain tumor segmentation using advanced techniques like mixed precision training and data pipeline optimizations. These enhancements significantly improve both computational efficiency and segmentation accuracy, enabling real-time clinical deployment.

---

## **Repository Outline**

- **`FinalProject.ipynb`**: Jupyter notebook with step-by-step implementation of the optimized U-Net model.
- **`README.md`**: This file, describing the project and providing instructions for execution.

---

## **Example Commands**

### **Running the Notebook in Google Colab**
1. Upload the notebook (`FinalProject.ipynb`) to Google Colab.
2. Enable GPU support:
   - Go to `Runtime` → `Change runtime type` → Select `GPU` under Hardware Accelerator.
3. Run each cell sequentially to:
   - Preprocess the dataset.
   - Train the U-Net model.
   - Evaluate the model's performance and visualize results.

---

## **Results and Observations**

### **Visualization**
- **Figure 1**: Model Predictions (Original Image, Ground Truth Mask, Predicted Mask)
- **Figure 2**: Training Metrics (Accuracy, IoU, Dice Coefficient, Loss)
  
![6c349cda-a71b-45d3-b1ab-b68006778ec2](https://github.com/user-attachments/assets/45e142c1-2fdf-4b83-902e-9eda4e6debb0)

![0e7507f8-7e60-45db-8826-5e9798164533](https://github.com/user-attachments/assets/2c704c40-6b02-4bd8-8c55-7cf163eebf9c)

### **Key Observations**
1. **Mixed Precision Training**: Reduced memory usage by leveraging float16 computations with float32 accumulations.
2. **Batch Size Doubling**: Enabled stable gradient estimation, improving generalization and GPU utilization.
3. **Data Pipeline Optimization**: Techniques like prefetching and parallelized augmentation minimized GPU idle time, reducing training time by about 50%.


---
