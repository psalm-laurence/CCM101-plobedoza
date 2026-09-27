# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system where the application and the database are separated into two parts. The application handles what the user sees and the requests they make, while the database is responsible for storing and managing the data.

## Web/Application Tier

The Web/Application Tier handles the user interface and user requests. In this activity, the Nextcloud container works as the application tier. It allows users to access and manage their private cloud storage through a web browser.

## Database Tier

The Database Tier is used to store the information needed by the application. In this activity, MariaDB works as the database for Nextcloud. It stores information such as user accounts, settings, and file-related data.

## Why Separate Them?

Separating the application and database into different containers makes the system easier to manage. Each container has its own purpose, so we can update, restart, or troubleshoot one container without directly affecting the other. This also makes the system more organized and easier to maintain.

