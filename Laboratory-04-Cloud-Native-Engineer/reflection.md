# Mission Reflection

This laboratory activity helped me understand why containers are becoming useful in cloud computing. Compared to installing a complete operating system on a Virtual Machine, starting a Docker container is much faster because the container uses the host operating system's resources instead of needing a separate guest operating system. In this activity, I was able to pull the Nginx image and run a web server with only a few Docker commands. This made the setup process feel much simpler and faster than setting up a traditional VM.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80, while I used port 8080 on the host machine to access it. The mapping connects the host's port 8080 to the container's port 80, allowing me to access the Nginx welcome page through `localhost:8080`.

When I use the `docker rm` command, the container itself is removed from Docker. Any data stored only inside that container can also be lost after the container is removed. This shows why important data should be stored using volumes or another form of persistent storage instead of keeping it only inside a temporary container.

I also learned that containerization can make collaboration between developers and IT operations easier. Developers can package an application with its required environment, while the operations team can run the same container without having to manually configure everything again. This supports the DevOps approach because both teams can work with a more consistent environment.

Finally, my GitHub portfolio is slowly becoming a collection of my actual laboratory activities and experiences. Each laboratory adds another project or skill that I can look back on and use as evidence of what I have learned in cloud computing.

