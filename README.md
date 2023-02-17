# Test Project

Task 1 - Dockerize the Application

The first task is to dockerise this application - as part of this task you will have to get the application to work with Docker and Docker Compose. You can expsoe the frontend using NGINX or HaProxy
The React container should also perform npm build every time it is built. Hint/Optional - Create 3 separate containers. 1 for the backend, 2nd for the proxy and 3rd for the react frontend
The only strict requirement is that the application should spin up with docker-compose up --build command


Task 2 - Deploy on Cloud

Next step is to deploy this application on AWS
At this point the application is already containerized, so you could deploy it to services which take an advantage of that fact, example ECS Fargate/EKS
The deliverable of this task is infrastructure as a code so we are interested in seeing the terraform/ansible files. We don't need to see the environment running but we will use your deliverable to try it out, so make sure it is easy for us to configure credentials etc..


Task 3 - Get it to work with Kubernetes

Next step is completely separate from step 2. Go back to the application you built in Task 1 and get it to work with Kubernetes.
Separate out the two containers into separate pods, communicate between the two containers, add a load balancer (or equivalent), expose the final App over port 80 to the final user (and any other tertiary tasks you might need to do)
Add all the deployments, services and volume (if any) yaml files in the repo. The only hard-requirement is to get the app to work with minikube