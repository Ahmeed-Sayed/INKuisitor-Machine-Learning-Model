# INKuisitor

## Offline Signature Verification Web Application System (Computer Systems Engineering Graduation Project 2021)


Offline Signature Verification model using deep learning methods to authinticate identity by  distinguishing between signatures.

The model have been created using One Shot Learning technique and a Siamese neural netowrk. One of the goals that we had in our minds before desigining the model was to not make the model language or regional exclusive. So, several datasets including multiple languages were used to train the model.

1) Data Acquisition 
        
For the datasets, the [ICDAR2011 (Dutch)](https://drive.google.com/file/d/1BPTu5uxwd4z6s17ius50NuqM3Fgb1owS/view?usp=sharing
), [Kaggle (English)](https://drive.google.com/file/d/13eRZTAxtiAjCURVZfOzqzUv_kZzgr8nr/view?usp=sharing
), [Cedar (English)](https://drive.google.com/file/d/1XY1k2o8E7FbAbqmdw7Cnjoky8fwF-t-V/view?usp=sharing
) and [BHSig260 (Bengali, Hindi)](https://drive.google.com/file/d/11xrkAxigGBoCDQ-lM4zII0VR3gy0R2sj/view?usp=sharing
) have been used to develop our model. 

2) Data Preprocessing [Code](https://nbviewer.jupyter.org/github/ahmedatef1610/INKuisitor-Machine-Learning-Model/blob/master/images_processing.ipynb
)
        
     1- Noise Removal: Gaussian blur technique was used to remove the noise in the dataset samples 
     ![image](https://user-images.githubusercontent.com/47431372/127754268-4c20a3db-0715-45bd-a2e4-1e218b14df92.png)
     ![image](https://user-images.githubusercontent.com/47431372/127754279-32ac43a2-9391-4b5f-b55b-59dd9d1e2938.png)
     
     2- Binarization
     
     ![image](https://user-images.githubusercontent.com/47431372/127754286-987361db-dbaa-493b-b5c2-d549cfc1716f.png)

     3- Finding Signature Contour 
     
     ![image](https://user-images.githubusercontent.com/47431372/127754325-b34b4f1f-bb14-472f-8943-1f8d6b402fdc.png)
     
     4- Signature Cropping and Resizing
     
     ![image](https://user-images.githubusercontent.com/47431372/127754335-57923015-4a15-4d41-a38d-29000c7f7758.png)
     
     5- Final Binraization 
     
     ![image](https://user-images.githubusercontent.com/47431372/127754348-ff7ffba8-38af-4440-9662-2aad36eb1a4e.png)



3) Model Architecture [Code](https://nbviewer.jupyter.org/github/ahmedatef1610/INKuisitor-Machine-Learning-Model/blob/master/project5.ipynb
)
  
Siamese network is considered as an implementation of One-Shot learning technique, it consists of parallel convolution networks, could be two or more.The model evaluates the two input images by finding the similarity score between the two images between 0 and 1 clarifying whether the test image is genuine or forged based on the similarity score.
  
  ![image](https://user-images.githubusercontent.com/47431372/127754404-d06d6270-f701-49bd-85de-2ddb22e9cedb.png)
  
  The CNN type used in this project is a Dense 201 type netowrk. 
  
  ![image](https://user-images.githubusercontent.com/47431372/127754468-d9336df1-e60b-4258-a327-ed8eb7fdc509.png)


4) Machine Learning Model's Block Diagram     

![image](https://user-images.githubusercontent.com/47431372/127754482-ba57877d-15a3-4418-8002-11601e9e9409.png)


5) Results and Evaluation [Code](https://nbviewer.jupyter.org/github/ahmedatef1610/INKuisitor-Machine-Learning-Model/blob/master/project6.ipynb
)

  
- The BHSig260 (Hindi) dataset gave accuracy of 84.53062248995984 %

![image](https://user-images.githubusercontent.com/47431372/127754644-d53a7c6c-e879-424d-8340-44b8ff34b47d.png)


- The BHSig260 (Bengali) dataset gave accuracy of 88.214859437751 %

![image](https://user-images.githubusercontent.com/47431372/127754641-3733f10b-2da9-49be-a5f7-abfb7ae6cfa2.png)


- The ICDAR2011 (Dutch) dataset gave accuracy of 89.49152542372882 %

![image](https://user-images.githubusercontent.com/47431372/127754638-db9430d8-49f4-4113-bcd5-ad5c06f4f2a4.png)


- The Kaggle (English) dataset gave accuracy of 89.80952380952381 %

![image](https://user-images.githubusercontent.com/47431372/127754636-e5499e2a-b841-49a7-9ede-07bac390260b.png)


- The Cedar (English) dataset gave accuracy of 89.29364063166881 %

![image](https://user-images.githubusercontent.com/47431372/127754634-8ca43cd1-fbaf-4212-9db0-5416deb4120e.png)



---

### [INKuisitor Backend](https://github.com/hossam507/INKuisitor-Backend)

### [INKuisitor Fronend](https://github.com/DevDerpi/INKuisitor-Frontend)
