
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

**Frontend**
```bash
vite (bundler-react)
tailwindcss (styling)
react-icons (icons)
react-router-dom (routing)
react-toastify (notify)
axios (API)
```
**Backend**
```bash
express (API)
jwt-token (token)
nodemail (MAIL)
bcrypt (encryption)
```

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/rudrax14/MERN_STACK-StudentTeacher-Booking-Appointment
    ```

2. **Install backend dependencies:**
    ```bash
    cd backend
    npm install
    ```

3. **Install frontend dependencies:**
    ```bash
    cd frontend
    npm install
    ```

4. **Set up environment variables for the backend:**

    Create a `.env` file in the `backend` directory with the following content:
    ```env
    DB_URL=''
    JWT_KEY = ''
    PORT = 5000

    # mail integration 

    MAIL_HOST = smtp.gmail.com
    MAIL_USER = 'your_mail'
    MAIL_PASS = 
    ```

5. **Run the backend server:**
    ```bash
    cd backend
    npm run dev
    ```

6. **Run the frontend server:**
    ```bash
    cd frontend
    npm run dev
    ```
7. **Set up environment variables for frontend:**

    Create a `.env.local` file in the `frontend` directory with the following content:
    ```env
    VITE_BACKEND_URL='http://localhost:5000'
    ``` 

The application should now be running on `http://localhost:5173/`.

## Usage

1. **Admin:**
    - Log in to the admin dashboard.
    - Add, update, or delete teachers.
    - Approve student registrations.

2. **Teacher:**
    - Log in to the teacher portal.
    - Schedule, approve, or cancel appointments.
    - Send email alerts to students.
    - View messages and all appointments.

3. **Student:**
    - Register and log in to the student portal.
    - Book appointments with teachers.
    - Send email alerts and messages to teachers.

## Screenshots

Landing Page 

![landingpage Dark](https://github.com/rudrax14/MERN_STACK-StudentTeacher-Booking-Appointment/assets/97178716/d3d4b1ef-e3ff-413e-afd4-3dabce321705)

Student Dashboard

![student dashboard dark](https://github.com/rudrax14/MERN_STACK-StudentTeacher-Booking-Appointment/assets/97178716/ab39e093-3bad-4101-982d-5eb459593580)

Teacher Dashboard

![teacher d Dark](https://github.com/rudrax14/MERN_STACK-StudentTeacher-Booking-Appointment/assets/97178716/ab56fb55-e38f-47d9-9622-0e48257d06e5)


Admin Dashboard

![admin ](https://github.com/rudrax14/MERN_STACK-StudentTeacher-Booking-Appointment/assets/97178716/5a3a856a-e26c-4e83-8179-1bb4da6ee810)



## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create your feature branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a pull request.

## Thank You 

**Keep Coding**

