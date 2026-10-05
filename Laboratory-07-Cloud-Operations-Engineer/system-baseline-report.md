# System Baseline Report

## Host System Baseline

Before deploying the client website, I checked the basic health of the Linux server to understand its available resources.

### Memory

The server has a total of **1.9Gi** of available RAM.

I used the following command:

```bash
free -h
```

### Disk Storage

The root (`/`) file system has a total storage capacity of **19G**.

I used the following command:

```bash
df -h /
```

### CPU and Processes

I used the following command to view active processes and CPU activity:

```bash
top
```

The command allowed me to observe the server's CPU usage and running processes in real time.

### Why Disk Space Is Important

Checking disk space before a massive traffic surge is important because applications need enough storage for logs, temporary files, cached data, and other system operations. If the disk becomes full, it can cause applications or services to stop working properly.
