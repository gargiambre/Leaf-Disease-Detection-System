# Leaf-Disease-Detection-System
Agriculture is the backbone of India. Tomato leaf disease detection employs technology to detect the diseases of tomato leaf when tomato leaf is uploaded and then the system will classify what kind of diseases the leaf has.This application will help farmers or peoples who love to grow plants detect the diseases as early as possible to save the plant from getting bad. Almost 65\% of Indian population relies on agriculture and farming. Hence, disease detection plays a vital role in reducing the degradation of agricultural products. As tomato is a vital vegetable in the Indian household, it is also the  second most often grown vegetable in India. The tomato plants are prone to diseases like late blight, septoria leaf spot, leaf mold, bacterial spot and, two spotted spider mites. Hence, implementing automatic disease detection's in agriculture can significantly improve the crop health and yield. Various researches have been conducted to overcome this  challenge. In this study an optimized Convolutional Neural Network (CNN) and You Look Only Once V8(YOLO) is introduced for early disease detection in tomato leaves. A dataset containing  images were taken which overcomes the limitations of under-fitting in existing models. The results show that the overall accuracy achieved by the model was 97\%. The results of our model shows that the proposed methodology can help farmers to detect tomato plant diseases at an early stage, thus prevents yield losses and improve overall growth productivity.

# Methodology
# 1) Image Acquisition: 
Image acquisition devices, this step includes use of upload image option provided in the interface of the application to upload the image of tomato leaf.
2) Image Pre-processing: Image pre-processing techniques in this step the captured image is being proceed as input and can be broadly classified into image enhancement and image restoration for the system. Pre-processes the input image then converts the input in interpolate grey level mapping to assemble the final image.
3) YOLO Model: Once the uploaded image gets pre-processed and matched with the dataset after that it goes to the next step that is YOLO (you only look once) algorithm which will identify and localize the region of interest which in this case would be the disease part of the leaf after identifying it will output the bounding boxes around that region indicating the presence of leaf diseases.
4) CNN Model: After figuring out the diseased part of the leaf with the help of YOLO. The Pre-trained CNN will then analyze the content within the bounding boxes to classify the detected regions into different disease categories. And will identify the specific type of disease present on the leaves.
5) Classification and Recognition:  Classification and Recognition stage. In this step the images that has been identified from the above stage will be classified with the tomato leaf diseases dataset and then it generates the output of the uploaded input image with the diseases name along with precautions to be taken such as pesticides and fertilizers to be used.


# Repository Content
dataset/: Contains the dataset of images used for training and testing.
api/: Includes the backend API for handling image uploads and processing.
frontend/: Provides the frontend interface for users to interact with the system.
models/: Holds trained models used for disease classification.
model1/, model2/: Additional models or variations used in the project.
cnn_and_yolo_based_plant_disease_detection.ipynb: Jupyter notebook containing code and explanations of the CNN and YOLO-based disease detection.
training/: Scripts or notebooks used for model training and evaluation.
