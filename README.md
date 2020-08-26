## Face-Mask-Detector

The project is based on live detection of person wearing a facial mask or not.
As we know we are living in time where wearing facial mask is necessary as well
as mandatory. Therfore it is required to detect if person is outdoors in a public area 
,is he/she wearing mask or not, as a concerns for the safety of the person and the others
too.

 



### Project Implementation:
*The project has 3 main parts:*

- Classification :  To classify b/w if the person wearing mask and person without mask
- Face detection: Detection of person Face in Image or a Live Video Frame
- Mask Prediction : Using Face(detected in previous step) as input detect if the person is wearing a mask or not.





### Project Structure:

There are total 4 python notebooks in the project:

- Classification_Pytorch_Tl: It is implementation of CNN classification using pretrained Resnet50 Model
- MaskPrediction_Pytorch_TL: Using the classification saved Model , testing the output on sample images
- MaskPredictionLive_using_OpenCv: Face detection using Haarcascade or Cv2.dnn library + mask prediction on live video frame.
- MaskPredictionLive_using_Facenet_Pytorch: Face detection using Facenet Pytorch + mask prediction on live video frame.

###### Samples 

This folder contains videos and images for Testing

###### facedetectionmodels

This folder contains pretrained models and haarcascades for Face Detection.





### Dependencies :

- PyTorch
- OpenCv
- Cuda -11.0
- Facenet-Pytorch





### How to Run and Visualize the output

If you want to see the Direct Results , Directly  run  "MaskPredictionLive_using_Facenet_Pytorch"

notebook.  This Approach give the best Results. All the outputs are generated using this notebook.



if you understand the complete flow of the Project follow the 

##### Step by Step Approach:

- ###### Create the Data:

  The data is not include in this repository due to large size. But the data i used was create manually. But u can use data used in this [article](https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/)

  The Data structure should be 

  ​			data/

  ​					train/

  ​							with_mask/

  ​							without_mask/

  

  With_mask should have images of the person  face with mask and Without mask should have images of the person face without Mask.

  I used around 200 images of each class and then applied following augmentations to create around 700 images of each class.

  Augmentations applied:  flip horizontal, rotate 45 ,rotate -45, blur, 

  

- ###### Run

  1. Classification_Pytorch_Tl
2. MaskPrediction_Pytorch_TL
  3. MaskPredictionLive_using_OpenCv   or MaskPredictionLive_using Facenet_Pytorch



### Output



https://github.com/kj5699/Face-Mask-Detector/blob/master/Outputs/ezgif.com-video-to-gif.gif



### References 

[PYimage search](https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/)

https://github.com/timesler/facenet-pytorch

https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html



















