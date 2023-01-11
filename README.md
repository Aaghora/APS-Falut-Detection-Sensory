Sensor-Fault-Detection
Problem Statement
```
The Air Pressure System (APS) is a critical component of a heavy-duty vehicle that uses compressed air to force a piston to provide pressure to the brake pads, slowing the vehicle down. The benefits of using an APS instead of a hydraulic system are the easy availability and long-term sustainability of natural air.

This is a Binary Classification problem, in which the affirmative class indicates that the failure was caused by a certain component of the APS, while the negative class indicates that the failure was caused by something else.

Solution Proposed
In this project, the system in focus is the Air Pressure system (APS) which generates pressurized air that are utilized in various functions in a truck, such as braking and gear changes. The datasets positive class corresponds to component failures for a specific component of the APS system. The negative class corresponds to trucks with failures for components not related to the APS system.

The problem is to reduce the cost due to unnecessary repairs. So it is required to minimize the false predictions.
```
```
Tech Stack Used
Python
FastAPI
Machine learning algorithms
Docker
MongoDB
Infrastructure Required.
AWS S3
AWS EC2
AWS ECR
Git Actions
Terraform
```
```
How to run?
Before we run the project, make sure that you are having MongoDB in your local system, with Compass since we are using MongoDB for data storage. You also need AWS account to access the service like S3, ECR and EC2 instances.
```
```
Data Collections
image

Project Archietecture
image

Deployment Archietecture
image
```

```
Step 1: Clone the repository
git clone https://github.com/sethusaim/Sensor-Fault-Detection.git
Step 2- Create a conda environment after opening the repository
conda create -n sensor python=3.7.6 -y
conda activate sensor
Step 3 - Install the requirements
pip install -r requirements.txt
Step 4 - Export the environment variable
export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>

export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>

export AWS_DEFAULT_REGION=<AWS_DEFAULT_REGION>

export MONGODB_URL="mongodb+srv://<username>:<password>@ineuron-ai-projects.7eh1w4s.mongodb.net/?retryWrites=true&w=majority"
Step 5 - Run the application server
python app.py
Step 6. Train application
http://localhost:8080/train
Step 7. Prediction application
http://localhost:8080/predict
Run locally
Check if the Dockerfile is available in the project directory

Build the Docker image

docker build --build-arg AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID> --build-arg AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY> --build-arg AWS_DEFAULT_REGION=<AWS_DEFAULT_REGION> --build-arg MONGODB_URL=<MONGODB_URL> . 

Run the Docker image
docker run -d -p 8080:8080 <IMAGE_NAME>
To run the project first execute the below commmand. MONGO DB URL:

mongodb+srv://avnish:XglZZ9OkjjUw74pZ@ineuron-ai-projects.7eh1w4s.mongodb.net/admin?authSource=admin&replicaSet=atlas-okvkrd-shard-0&w=majority&readPreference=primary&appname=MongoDB%20Compass&retryWrites=true&ssl=true
windows user

MONGO_DB_URL=mongodb+srv://avnish:XglZZ9OkjjUw74pZ@ineuron-ai-projects.7eh1w4s.mongodb.net/admin?authSource=admin&replicaSet=atlas-okvkrd-shard-0&w=majority&readPreference=primary&appname=MongoDB%20Compass&retryWrites=true&ssl=true
Linux user

export MONGO_DB_URL=mongodb+srv://avnish:XglZZ9OkjjUw74pZ@ineuron-ai-projects.7eh1w4s.mongodb.net/admin?authSource=admin&replicaSet=atlas-okvkrd-shard-0&w=majority&readPreference=primary&appname=MongoDB%20Compass&retryWrites=true&ssl=true
then run

python main.py
```

```bash
pip install -r requirements.txt
```

### Step 2 - Run main.py file

```bash
python main.py
```
```
git (Enter)   #checking if git is installed
```
git --version #Checking version
```
```
wget + link #to download the data in mgdb
```
```
git remote -v #to check if other git repo is linked
```
```
git remove remove origin  #to disconnect a git repo connected with project
```
```
git log #gives logs of all version and action taken on git
```
