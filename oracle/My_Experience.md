# Oracle User Assistant Devloper Technical Assessment 

**MY EXPERIENCE** 

In this exercise, I need to run the TODO list manager application that's running in Node.js , which was a sample containerized application on Official Docker documentation.

***Steps That I Followed***
 1.I followed the instructions as mentioned in the email for installing Docker. After installing Docker on Windows 11 and completing all of the Docker installation steps.
 2. I followed the official Microsoft documentation on WSL (Windows Subsystem for Linux). I downloaded WSL using the command `wsl --install` and set the default version using the command `wsl --set-version 2` on Command Prompt, which was required for Docker to be run on Windows.
 3. Then I downloaded the same Github repository mentioned in the documentation for containerizing the application, since it was a backend repostory , and unpack the Zip file for further procedures.
 4. In order to build the container image I created a dockerfile in the app directory of unpacked file i.e getting-started-master using the command `type nul > dockerfile` then implemented it using VS Code and finalised it with `docker build -t getting-started .`command .
 5. All the above mentioned steps led me to create a container image in Docker that was used to run the sample backend TODO manager application.
 6. To start the container application, I followed all the direct commands and instructions as mentioned in the official documentation, and then ran the application from Docker and was able to perform all the operations in application that was hosted over on local host 3000 server.
 
 
***Troubleshooting*** 
While opening the Docker , it displayed the Docker starting error i.e Docker was stuck and still in start-up mode because , by default, it is using Hyper-V configuration when it needs to be run on WSL(Window Subsytem For Linux) version 2 backend.
For the ***Improvements*** of the procedure that was mentioned in official documentations , it can be more impressive for window users if WSL 2 backend installation commands already mentioned as a steps after the Docker installation to properly setup the Docker application and enabling the VM feature from Window Features is also required that can also be mentioned as a step in documentation.

***My Learnings From This Exercise***
The overall official documentation and tutorial were quite easy and explained well enough that even beginners could run the application or deploy the repository on a local host using the Docker container.

Docker is an open platform for developing, shipping, and running applications , Docker’s methodologies for shipping, testing, and deploying code quickly, it can significantly reduce the delay between writing code and running it in production. 
For effectively running of the Docker application it is required to have pre-installed WSL(Windows Subsystem for Linux).
WSL generally runs Linux applications, utilities, and Bash command-line tools directly on Windows, unmodified, without the overhead of a traditional virtual machine or dual-boot setup.  Then I learned about container, which is a runnable instance of an image. It can create, start, stop, move, or delete a container using the Docker API or CLI. Container uses an isolated filesystem provided by a container image , container image contain everything needed to run an application - all dependencies, configurations, scripts, binaries, etc. We can directly send the container image to another computer to run the application on another server.

To ***Approach*** This type of procedure for maintenance and deployment of applications requires that proceed with the official documentation and follow all the steps and instructions provided or mentioned for that particular procedure for deploying and maintaining applications like this , if any features or steps are missing, they can be found on websites like Stack Overflow, Guru, Bloomfire, etc.

A tool like Docker deploys multiple containers,  it places applications in virtual containers that run on the same operating system. It is mainly used as a software development platform for developing distributed applications that work efficiently in different environments.
To deploy any application like this on Docker : These steps should be followed
1. Build images 
2. Run your image as a container.
3. Use containers for development.
4. Run tests.
5. Deploy your app.

Docker can be used to deploy different type of application , we can deploy react application , Node.js applications , etc,
There are different types of containerized applications that can be used as alternatives to Docker; Kubernetes and Amazon Elastic Container Service (ECS) are examples of popular container orchestration tools.

 
 


