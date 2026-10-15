# Reflection

This activity helped me understand why automation is important when managing hundreds of cloud servers. Performing the same task manually on every server would take a lot of time and could lead to mistakes. With scripts and scheduled tasks, administrators can repeat tasks more consistently and spend more time monitoring systems and solving other problems.

However, automation also has risks. If a script contains a destructive command or a serious typo, it could damage files or affect many servers if it runs everywhere. For example, a mistake in a script deployed to 1,000 servers could cause widespread data loss or service interruptions. This is why scripts should be tested carefully, reviewed by other people when appropriate, and given only the permissions they need before being deployed on a large scale.

Writing a Bash script was different from creating a Docker Compose YAML file in Mission 6. A Bash script contains commands that run step by step to perform tasks, such as creating directories and compressing files. Docker Compose uses YAML to describe services, containers, and their configurations. Bash focuses on executing commands, while Docker Compose defines how an application environment should run.

Looking back at the activities from Laboratory 1 to Laboratory 9, my understanding of cloud computing has improved. I started by learning basic Linux commands and system information. Later, I worked with virtual machines, containers, storage, deployment, monitoring, and security. In this activity, I learned how automation connects with those skills and helps make cloud operations more efficient.

The role I enjoyed most was the Cloud-Native Engineer because working with Docker and deploying applications helped me understand how containers make software easier to run and manage. I also found the security and automation activities useful because they showed me how to protect applications and reduce repetitive work. Overall, these missions helped me become more confident using Linux and understanding the tasks involved in managing cloud environments.
