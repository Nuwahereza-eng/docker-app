This Repo is a simple website and it contains a dockerfile which can be executed to create a docker image .
It is my first project implementing containerization using docker.
HOW TO RUN THIS PROJECT USING DOCKER
Step 1: Clone the repository
Clone the repository to your local machine:
On your CLI
git clone https://github.com/Nuwahereza-eng/docker-app.git
cd docker-app
Step 2: Build the Docker Image
Navigate to the project directory and run the following command to build the Docker image:

docker build -t my_website .
This will create a Docker image named my_website based on the instructions in the Dockerfile.

Step 3: Run the Docker Container
Once the image is built, you can run the container using the docker run command:

docker run -d -p 8080:80 my_website
This command will:
Run the container in detached mode (-d).
Map port 80 of the container to port 8080 on your local machine (-p 8080:80).
You can now open your web browser and visit http://localhost:8080 to view the website.

Run the following command to start the web service:

docker-compose up -d
This will use Docker Compose to build and run the containers, and you can access the website at http://localhost:8080.

To stop and remove the containers, run:

docker-compose down

