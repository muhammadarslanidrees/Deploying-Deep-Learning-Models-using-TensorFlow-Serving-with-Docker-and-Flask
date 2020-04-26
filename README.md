# Deploying-Deep-Learning-Models-using-TensorFlow-Serving-with-Docker-and-Flask
In this project, we will deploy a Pre-trained TensorFlow model with the help of TensorFlow Serving with Docker, and we will also create a visual web interface using Flask web framework which will serve to get predictions from the served TensorFlow model and help end-users to consume through API calls. 

Execution Steps: 
  1.  Setting up tensorflow serving server on localhost:
  
			1. RUN CMD as administrator and execute the below command
			2. docker run -p 8501:8501 --name=pets -v "C:\pets:/models/pets/1" -e MODEL_NAME=pets tensorflow/serving
  
  2.  Setup virtual environment and installing flask and its dependencies: 
  
      1. 	Conda create –n flaskapp python=3.7
		  2.  Conda activate flaskapp
		  3.  pip install tensorflow==2.1.0 flask flask-bootstrap requests pillow
		  4.  Python app.py
      5.  Access the app by going to localhost:5000 in your browser
      
Assumptions are that you’re running Windows with python 3.7

Ref: https://www.coursera.org/projects/deploy-models-tensorflow-serving-flask
