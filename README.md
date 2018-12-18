# FaceRecognition
Captures images from your webcam video stream Extracts all Faces from the image,Recognise Faces


	FaceRecognition/face recog/face_data_collect.py


Python Script that captures images from your webcam video stream
Extracts all Faces from the image frame (using haarcascades)
Stores the Face information into numpy arrays

 1. Read and show video stream, capture images
 2. Detect Faces and show bounding box (haarcascade)
 3. Flatten the largest face image(gray scale) and save in a numpy array
 4. Repeat the above for multiple people to generate training data


	    FaceRecognition/face recog/face_recognition.py
      
 Recognise Faces using some classification algorithm - like Logistic, KNN, SVM etc.


 1. load the training data (numpy arrays of all the persons)
		# x- values are stored in the numpy arrays
		# y-values we need to assign for each person
 2. Read a video stream using opencv
 3. extract faces out of it
 4. use knn to find the prediction of face (int)
 5. map the predicted id to name of the user 
 6. Display the predictions on the screen - bounding box and name



		FaceRecognition/face recog/haarcascade_frontalface_alt.xml
 
trained haarcasecade for frontalface   
download from 

https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_alt.xml
      



