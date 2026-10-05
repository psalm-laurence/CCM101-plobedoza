# Laboratory 07 - The Cloud Operations Engineer

## Mission Overview

Congratulations! Your ability to deploy multi-tier architectures has proven your technical capabilities. You have now been promoted to the Cloud Operations Team (often referred to in the industry as Site Reliability Engineering, or SRE) at CloudNova Technologies. Deploying a cloud application is only the first step; keeping it running smoothly is the real challenge. When a server crashes or a web page takes ten seconds to load, you cannot simply guess what is wrong. You 
must rely on Observability and Monitoring to see inside your infrastructure. Using the KillerCoda Playground, you will step into the role of a Cloud Operations Engineer. You will establish a performance baseline for your Linux server, deploy a containerized application, generate artificial web traffic, and hunt down performance metrics and system logs to prove the application is healthy. 

## Objectives
At the end of this laboratory activity, you should be able to: 
* Utilize native Linux command-line tools to monitor host CPU, Memory, and Disk capacity. 
* Deploy a web container and track its real-time performance using Docker metrics. 
* Generate web traffic and extract application access logs for analysis. 
* Translate raw performance data into a readable technical report using Markdown. 
* Continue expanding a professional GitHub Cloud Computing Portfolio. 

## Monitoring Commands Executed

```bash
free -h
df -h /
top
docker run -d -p 8080:80 --name client-website nginx
docker ps
curl http://localhost:8080
curl http://localhost:8080/hidden-admin-page
docker logs client-website
docker stats
```

## Skills Learned

Through this activity, I learned how to check the basic health of a Linux server and monitor a running Docker container. I also learned how to generate test web traffic, read application logs, and check real-time CPU and memory usage. These skills helped me understand how Cloud Operations Engineers use observability to troubleshoot and monitor applications.
