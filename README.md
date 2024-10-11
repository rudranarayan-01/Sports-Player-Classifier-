
# SPORTS PLAYER CLASSIFICATION ML PROJECT 

This is an end to end project on Image classification where our end goal is to build a website where you can drag and drop an image of a sport person and it will identify that sport person. Here we have taken only five sport persons to do image classification. We will build a model first, hyper tune it, exported to a file, then we will run a python flask server and our website will make a call to that python flask server. From our website we drop an image of Sport person to identify his/her name.

## Different Steps
This Sports Person Classification project carries different steps :

- Gather and Scrape Sports Person Data
- Data cleaning using Haar Cascade from OpenCV
- Feature Engineering using Wavelet Transforms
- Model building
- Create Python Flask server
- Build a Website


## System Modules

### Step 1: Gather and Scrape Sports Person Data
Gather and Scrape data is done by different ways like we can Manually Download Image from Google, Using Python and Web scrapping, Buy Data from third party vendors or Fatkun Chrome Tool. For our project we have collected data using Fatkun Chrome Tool, it download images from web and you can also filter the images based on width.

### Step 2: Data cleaning using Haar Cascade from OpenCV
After gathering all images we want to detect if the face in the image is clearly visible or not and for that you will try to detect a face with two eyes. If the face and eyes are clearly visible then we will keep that image otherwise we will discard it. For face detection and the eyes detection we are using Haar Cascade from OpenCV which is a famous image processing library in Python.

### Step 3: Feature Engineering using Wavelet Transforms
The wavelet transform is a tool that cuts up data, functions or operators into different frequency components, and then studies each component with a resolution matched to its scale. In wavelet transformed image, you can see edges clearly and that can give us clues on various facial features such as eyes, nose, lips etc. In our case we are doing a sports celebrity classification only for five players which are, Kohli, Roger Federer Serena, Williams Liana, Messi and Maria sharapova.

### Step 4: Model building
Used SVM with linear kernel tuned with fine tuning for Model building. We tried support vector machine because vector machine tends to perform good when it comes to classification then we also tried couple of other models using GridSearchCV.

### Step 5: Create Python Flask Server
Python Flask Sever use exported pickle file and JSON file, it does the actual image classification. This flask server is used as a back end for UI application. when you drag and drop image on the UI, UI will convert it to base64 string and send it to back-end, So to use that image back-end needs to convert it.

### Step 6: Build a Website
On website UI we drag and drop the image on the Drop Zone and when it send this image to back-end, Python Flask Sever will use that image for the classification. We are going to build a website or UI or a front-end for our sport persons classifier project we will be using a simple HTML, CSS, JavaScript to build the UI which will make HTTP call to our back-end using j Query.

## Tech-Stack-Used
 We have classify the whole project into three directories 
    - model
    - server
    - UI

**Frontend**
```bash
HTML
CSS
JS
Jquery
```
**Backend Server**
```bash
flask
numpy
base64
wavelet
```

**Model**
```bash
 pandas
 cv2
 matplotlib
 Python Wavelet
 sklearn
 seaborn
 joblib
 json
```

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/rudranarayan-01/Sports-Player-Classifier-
    ```

2. **Install backend dependencies:**
    ```bash
    cd server
    python server.py
    ```

## Screenshots

Landing Page 

(![Screenshot 2024-10-10 132216](https://github.com/user-attachments/assets/08012f03-93a7-48a3-b801-3a3ab44b79d0)
)




## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create your feature branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a pull request.

## Thank You 

**Keep Coding**

