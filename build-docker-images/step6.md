Once the build has completed you should see the Image and Tags using the Docker CLI `docker images`{{execute}}.

What was built into the Docker Image was a small HTTP server. You can launch it using:
`docker run -d -p 80:80 katacoda/jenkins-demo:latest`{{execute}}

Using cURL you should see the server respond:
`curl docker`{{execute}}

Jenkins will have the console output of our build, available via the dashboard. You should be able to access it below:

https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/job/Katacoda%20Jenkins%20Demo/1/console

If you rebuilt the project, you would see a version 2 image created and the _:latest_ tag reattached.
