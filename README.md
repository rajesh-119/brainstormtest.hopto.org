# Automated Deployment of a WordPress Website

This repository contains the code and configuration files for automating the deployment of a WordPress website using Nginx, LEMP stack, and GitHub Actions. The deployment process follows security best practices and ensures optimal performance of the website.

## Table of Contents

- [Introduction](#introduction)
- [Server Provisioning](#server-provisioning)
- [Securing the VPS](#securing-the-vps)
- [Installing and Configuring LEMP Stack](#installing-and-configuring-lemp-stack)
- [WordPress Installation](#wordpress-installation)
- [SSL/TLS Certificate Setup](#ssl-tls-certificate-setup)
- [GitHub Repository Setup](#github-repository-setup)
- [GitHub Actions Workflow](#github-actions-workflow)
- [Local Environment Setup](#local-environment-setup)
- [Deployment Instructions](#deployment-instructions)
- [Installation Guide](#installation-guide)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This deployment project automates the setup and maintenance of a WordPress website hosted on a Virtual Private Server (VPS) using Nginx, LEMP stack, and GitHub Actions.

### Goals and Objectives

- Efficiently provision and configure a VPS.
- Secure the server following best practices.
- Install and configure Nginx, MySQL, PHP, and WordPress.
- Implement SSL/TLS encryption for secure communication.
- Automate deployment using GitHub Actions.
- Optimize server performance for the WordPress website.

### Target Audience

This project is intended for developers, system administrators, or anyone looking to automate the deployment of a WordPress website with Nginx, LEMP stack, and GitHub Actions.

## Server Provisioning

### Provisioning a Virtual Private Server (VPS)

- Provision a VPS with a major cloud provider (e.g., AWS, Azure, Google Cloud, or DigitalOcean).
- Create a new VM instance with the desired specifications (e.g., t2.micro) and install Ubuntu 22.04.
- Configure security groups to allow SSH, HTTP, and HTTPS traffic.

### Securing the VPS

- Set up SSH access and connect to your VPS securely.
- Update the system and upgrade installed packages.
- Implement firewall rules using UFW to restrict access.

## Installing and Configuring LEMP Stack

- Install and configure Nginx as the web server.
- Install MySQL server and set the root password.
- Install PHP-FPM and PHP-MySQL.
- Configure MySQL for the WordPress database.

## WordPress Installation

- Create a directory for the website and set ownership to the web server user.
- Download and extract WordPress.
- Configure WordPress by copying the sample configuration file.

## SSL/TLS Certificate Setup

- Install Certbot and request Let's Encrypt certificates.
- Configure Nginx for HTTPS by editing the Nginx server block.

## GitHub Repository Setup

- Initialize a Git repository for your website files.
- Create a new repository on GitHub.
- Connect your local repository to GitHub.
- Push your code to the GitHub repository.

## GitHub Actions Workflow

- Create a `.github/workflows` directory in your repository.
- Add a YAML file for GitHub Actions to define the CI/CD workflow.
- Configure steps to install dependencies, build the project, and deploy to the server.
- Ensure you add your server's SSH key as a GitHub repository secret.

## Local Environment Setup

Before deploying to the server, you can set up a local development environment to test changes.

- Clone the GitHub repository to your local machine.
- Install any necessary development tools and dependencies.
- Configure your local environment to match the server environment.

## Deployment Instructions

To deploy your WordPress website to the VPS using GitHub Actions, follow these steps:

1. Push changes to your GitHub repository.
2. GitHub Actions will automatically trigger the deployment workflow.
3. The workflow will SSH into the server, pull the latest changes, and update the website.

## WordPress Website URL

You can access the deployed WordPress website at the following URL: https://brainstormtest.hopto.org/wp-admin/

## Installation Guide

For detailed installation instructions and step-by-step guidance, please refer to our [installation guide](https://docs.google.com/document/d/1YIGjGEVdtkTd0UBxaefotTMrb8dXC4GNWKc-97qvJ5I/edit?usp=sharing).

The installation document covers the following topics:

- Server provisioning
- Securing the VPS
- Installing and configuring the LEMP stack
- WordPress installation
- SSL/TLS certificate setup
- GitHub repository setup
- GitHub Actions workflow setup
- Local environment setup

## Contributing

Contributions to this project are welcome! If you have improvements or suggestions, please create a pull request.

## License
