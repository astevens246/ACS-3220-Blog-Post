# Deploying a News API: My Journey with Docker, CapRover, and Uptime Monitoring

Introduction
In this blog post, I want to share how I set up a News API using tools like Docker, CapRover, UptimeRobot, and DigitalOcean. This project helped me learn a lot about deploying and monitoring applications.

Here is a screen shot of my homepage: 

![News API Deployment](./images/Screen%20Shot%202024-10-10%20at%2010.11.01%20AM.png)


Project Overview
The News API lets users fetch, create, update, and delete news stories. I built this project to learn about RESTful APIs and get hands-on experience with deployment tools.

## Technologies Used

- **Docker**: Helps package applications so they run the same everywhere. [Learn more about Docker](https://www.docker.com/why-docker)
- **CapRover**: Makes it easy to deploy and manage applications. [CapRover Documentation](https://caprover.com/docs/)
- **UptimeRobot**: Checks if my application is running and sends alerts if it goes down. [UptimeRobot Features](https://uptimerobot.com/)
- **DigitalOcean**: Provides cloud servers to host my application. [DigitalOcean Overview](https://www.digitalocean.com/)

## Deployment Process

  I made a `Dockerfile` and `docker-compose.yml` to set up my application’s environment. Docker helped me package everything needed for my app to run smoothly.

### Creating the Docker Environment

1. **Dockerfile**: Defines the environment for the application.
2. **docker-compose.yml**: Manages multi-container Docker applications.

Deploying with CapRover
  Deploying to CapRover was simple. Here’s what I did:
   1. Installed the CapRover CLI.
   2. Logged into my CapRover server.
   3. Created a new app and deployed my Docker container.
   4. Set up environment variables for my database.

# Install CapRover CLI
npm install -g caprover

# Login to CapRover server
caprover login

# Create a new app
caprover deploy

   Configuring Uptime Monitoring
   To keep my application running, I used UptimeRobot to monitor it. I set up a monitor and alerts to let me know if my app went down. Monitoring is important to keep services reliable.

   Setting Up UptimeRobot
      1. Create an account on UptimeRobot.
      2. Add a new monitor for your application.
      3. Configure alert contacts to receive notifications.
   Uptime Robot Setup Guide: https://uptimerobot.com/blog/status-pages-guide/
   
   Challenges and Solutions
   I faced some challenges, like setting up the database connection and making sure my Docker containers talked to each other. By checking the logs and reading the documentation, I was able to fix these issues.

  Key Learnings:
   From this experience, I learned:
   - How important containerization is for consistent deployments.
   - How to use CapRover for easier application management.
   - The value of monitoring uptime to keep services reliable.
   - Tips for troubleshooting deployment problems.


   Deploying my News API with these tools was a great experience. I encourage others to try Docker, CapRover, and UptimeRobot for their projects. These tools make deployment easier and improve application reliability.

   Check out my [GitHub repository](https://github.com/astevens246/news-api) to see the project. Feel free to share your thoughts or ask questions in the comments!
```
