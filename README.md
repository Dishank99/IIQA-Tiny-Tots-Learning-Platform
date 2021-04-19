# IIQA-Tiny-Tots-Learning-Platform
IIQA (Interactive Image Question Answering) is Learning Platform for toddlers where they can attemp and learn from Image based quiz which are auto generated or can be generated by a Teacher using Virtual Classroom feature.

IIQA is a Web Application with the features of online classroom, automatic image based quiz generation. The User Interface has been built using a JavaScript library called ReactJS. The application is backed by Google Firebase for data and file storage. It will be having separate portals for Student and Teacher. Student portal will be having features of class-based learning, where they can join a particular class and attempt a quiz assigned by their respective Teacher and self-learning, where they can select an image module according to the category and attempt the quiz generated from the same. In Teacher’s portal, a Teacher can create a class, set up a quiz by providing image or selecting from the pre-defined modules provided and assign it to the Students of classroom. The quiz will be multiple choice based, along with a feature of text to speech so that Student can also listen to the question and options.
 For generation of quiz from images, we have used Visual Question generation (VQG) and Visual Question Answering (VQA). Both these techniques are amalgamation of Deep Learning domains - Computer Vision and Natural Language Processing. Visual Question Generation serves the purpose of generating question from the image and Visual Question Answering generates the answer for the given image and question generated. In our Application we are using both these methodologies in sequential manner. At first, question will be generated for the image using Visual Question Generation technique and then, that question along with the image will be further processed to generate answer using Visual Question Answering technique. A REST Webservice is built that will be using these methodologies and to serve question answer pairs along with options for the provided set of images. Hence, a quiz will be created.

## IIQA Application Architecture
![Application Architecture](https://github.com/Dishank99/IIQA-Tiny-Tots-Learning-Platform/blob/master/Final%20Application%20Arch.%20draft2.png)

#### IIQA Architecture has 3 primary components as given below with respective github link:
* IIQA UI - ReactJS App (https://github.com/anshuul/iiqa)
* IIQA Server as a substiture for Google Cloud Functions - NodeJS / ExpressJs (https://github.com/Dishank99/iiqa-server)
* IIQA AI Service - Python Flask / Keras / Tensorflow (https://github.com/Dishank99/Automatic-Image-Based-Question-Answer-Pair-Generator)
