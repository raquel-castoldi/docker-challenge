# docker-challenge-template

## Challenge 1

### Steps Taken
1. Established the "public" folder as per project requirements.
2. Crafted an "index.html" file within the "public" folder containing necessary personal information.
3. Developed a Dockerfile within the challenge1 directory.
4. Built the Docker image using the command `docker build -t my-nginx-image .`.
5. Ran the Docker container using `docker run --name my-nginx-container -d -p 8080:80 my-nginx-image`, ensuring appropriate port mapping.
6. Verified the application's functionality by accessing `http://localhost:8080` and confirming the correct display of "index.html".
7. Documented the process with screenshots of the terminal and result for reference.

## Challenge 2

### Steps Taken
1. Downloaded and extracted the challenge2 zip folder.
2. Created a Dockerfile within the directory and included necessary code for container building.
3. Formulated a docker-compose.yml file to handle Docker setup for the challenge.
4. Addressed and resolved multiple encountered mistakes through careful troubleshooting and adjustments.
5. Added a default.conf file with specific Nginx server configurations.
6. Rectified conflicts and errors encountered during `docker-compose up --build`, ensuring seamless deployment.
7. Confirmed successful completion by accessing `localhost:3000/api/books` in the browser.
8. Documented the process with screenshots of the terminal and result.

## Challenge 3

### Steps Taken
1. Downloaded and extracted the challenge3 zip folder.
2. Reviewed existing Dockerfiles and "nginx.conf" to understand the structure and connections.
3. Created a Docker Compose File (docker-compose.yml) to link Nginx, Node.js, and MariaDB services.
4. Addressed errors during environment setup through thorough testing and configuration adjustments.
6. Successfully rebuilt containers using `docker-compose up --build`, ensuring proper functioning on port 8080.
7. Verified the full stack functionality by accessing endpoints in the browser (`localhost:8080/api/books`, `localhost:8080/api/books/1`).
8. Documented the process with screenshots of the terminal and result.

## Challenge 4

### Steps Taken
1. Utilized the existing setup from Challenge 3, comprising Nginx, Node.js, and MariaDB.
2. Confirmed the operation of a single instance of node-service.
3. Scaled node-service from one to three instances by adding `deploy: replicas: 3` to the api section in services in the docker-compose.yml file
5. Verified scaling by observing different hostnames in responses to GET requests.
6. Confirmed all three instances of node-service were running using `docker-compose ps`.
7. Demonstrated successful load balancing by repeatedly accessing the `/api/stats` endpoint.
8. Documented the process with screenshots of the terminal and result.

## Conclusion
These challenges provided invaluable learning experiences, enhancing understanding of Docker and its practical applications. The hands-on approach facilitated a deeper comprehension of containerization concepts and their implementation.
