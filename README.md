# Dockerised Calculator Microservice

## Overview
This project is a basic calculator microservice I built using Node.js and Express, and then Dockerised it as part of the SIT323 5.1P task.  
The microservice can do simple operations like addition, subtraction, multiplication, and division through API endpoints.


### Step 1 - Basic App
First, I created a simple Node.js application (`index.js`) that can handle basic calculator operations through different endpoints.

### Step 2 - Create Dockerfile
Then, I wrote a `Dockerfile` to containerise the app.  
In the Dockerfile:
- I used the `node:18` image.
- Set the working directory to `/app`.
- Installed dependencies.
- Exposed port 3000.
- Set the start command to run `index.js`.

### Step 3 - Create Docker Compose File
After that, I made a `docker-compose.yml` file to make running the container easier.  
In the Compose file:
- I built the image directly from the Dockerfile.
- Mapped port 3000 on my machine to port 3000 in the container.

### Step 4 - Build and Run
To build and run everything, I used:

```bash
docker-compose up --build

### Step 5 - Testing
Once it was running, I opened the browser and tested the API endpoints like:
- `http://localhost:3000/add?num1=5&num2=3`
- `http://localhost:3000/subtract?num1=10&num2=2`
- `http://localhost:3000/multiply?num1=4&num2=5`
- `http://localhost:3000/divide?num1=8&num2=2`

### Step 6 - Push to GitHub
Finally, I pushed all the files to my GitHub repo:
```
https://github.com/Sanindu-Rukshan/sit323-2025-prac5p.git
```


```



---
