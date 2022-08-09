# Anomaly_Detection

problem overview:
      
      - Anomalies data can affects on the result of the machine learning models and every system, so we need 
        to define the anomalies data, because anomalies data are outliers are different from the right data.

      - So, we can use four algorithms for anomaly detection:
      
            1- KNN model.
            
            2- SVM model.
            
            3- PCA.
            
            4- DBSCAN

Implementation steps:
        
        - PyCaret anomaly detection module provides several pre-processing features that can be 
          configured when initializing the setup through setup function. 
        
        - It has over 12 algorithms and a few plots to analyze the results of anomaly detection. 
        
        - PyCaret's anomaly detection module also implements a unique function tune_model 
          that allows you to tune the hyperparameters of the anomaly detection model 
          to optimize the supervised learning objective such as AUC for classification or R2 for regression.

        1- Read the dataset without label.
        
        2- visualize the data using TSNE.
        
        3- Apply SVM model.
        
        4- TSNE plot in 2D (0 is not anomaly, 1 is anomaly) and umap.
        
        5- 3D TSNE Plot for outliers.
        
        6- Plot SVM model results along the data.
        
        7-Model evaluation for SVM.
        
        8- Apply KNN model.
        
        9- Model evaluation for KNN.
        
        10- Evaluate the dataset that has labels.
        
        11- show only the data that has label=1.
        
        12- Apply PCA model.
        
        13- Apply DBSCAN Model.
        
        14- delete the noise mapping -1 to 1 as anomely.
        
  
Conclusion:
        
        - After applying the four models and evaluating them, we notice that the accuracy differs 
          between the 4 models, so the accuracies are shown in the following tables:
          
          
  ![image](https://user-images.githubusercontent.com/54502733/183566763-2682defc-ed2d-4ad3-8414-b908ae52eaf4.png)
  
  
  ![image](https://user-images.githubusercontent.com/54502733/183566790-3c566f11-d735-4c4f-bfb6-a2a01bbb9283.png)



       - So, the best model to be used in anomaly detection according to the accuracies is the DBSCAN
         model, because it depends on denisty, but it needs to tune epsilon and minpoints.
         And the worst model according to the accuracies is KNN model
