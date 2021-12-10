# Real_Time-Face_Recognition-using-Haarcascade_Classifier-and-Face_Recognition

Using face-recognition 1.3.0 and Harrcascade_Classifier
Install face_recognition library using this commad 
"! pip install face-recognition " may you can follow this link for further details: " https://pypi.org/project/face-recognition/ "

Importing required libraries
import numpy as np
import cv2,os
import face_recognition

Importing haarcascade_classifier, you have to download it first and give its exact location 

face_cascade = cv2.CascadeClassifier('./model/haarcascade_frontalface_default.xml')

This funcation is comparing face with the images placed in Images folder by using different funcations of face_recognition 

Capturing video from Webcam.If you wants to use an external camera you have to give 1 instead of 0 in parameter

cap = cv2.VideoCapture(0)

Detecting face from frames using haarcascade classifier, Croping and saving the image of face in testing_images folder.If there is a image in testing_images folder then call face_rec funcation and if the face get detected it will show wellcome
