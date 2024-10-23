practical: push and pull
1.  Create repository in github
2.  Copy the HTTPS repo link provided by github
3.  Create a folder with txt file in the folder
4.  Open the folder with cmd
5.  git init
6.  git branch -M main
7.  git remote add your copy link
8.  git add filename.txt
9.  git commit -m "any message"
10.  git push -u origin main
11.  git pull origin main

DOCKER: To create Docker containers of any web application image.
1. Create getting-started-app folder.
2. open the cmd in the created folder
3. git clone https://github.com/docker/getting-started-app.git
4. cd getting-started-app
5. create an file as docker file
6. Using a text editor or code editor, add the following contents to the
Dockerfile:
# syntax=docker/dockerfile:1
FROM node:18-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000
7. docker build -t getting-started .
8. docker run -dp 127.0.0.1:3000:3000 getting-started
9. http://localhost:3000/
