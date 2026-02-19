# CST8915 Lab4: Introduction to Docker

**Student Name**: Bosi Chen\
**Student ID**: 041040774\
**Course**: CST8915 Full-stack Cloud-native Development\
**Semester**: Winter 2026

---

## Demo Video

🎥 [Watch Demo Video](https://youtu.be/BVeI6Lk9PZc)

---

## Reflection Questions

1. What are the main differences between a Docker image and a Docker container?
   
   The container is an environment in which the services are running, while the image is a template for creating a container.
   
2. Explain how Docker's layered architecture improves efficiency.
   
   Each layer is representing a set of filesystem difference. An image is formed by multiple layers stacking on top of eachother. This layered structure makes it easy to reuse the base layers shared by different images, and also minimizes the storage by storing the shared layers only once. 
  
3. Why does each container get its own writable layer?
   
   This temporary layer allows the container to modify, create, or delete files without affecting the original image, which should be immutable.
   
4. What are the benefits of using Docker Compose over running containers individually?

   When you have an application with multiple Docker service to run, it is easier to orchestrate the Docker images using a Docker Compose together.

---

## Challenges

At first I created a VM with 1GB RAM, this VM will crash and need to restart when building the docker images and starting the services. I need to swith to another one of 4GB RAM to let it build and run smoothly.
