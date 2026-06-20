# Task 1: AWS S3 Static Portfolio Website Hosting

## Project Overview

This project demonstrates how to host a personal portfolio website using AWS S3 Static Website Hosting without provisioning any servers.

The portfolio was originally developed using React, TypeScript, and Vite. A production build was generated using `npm run build`, which converted the application into static HTML, CSS, and JavaScript files. These files were then deployed to an AWS S3 bucket and made publicly accessible through a website endpoint.

## Objective

* Create a personal portfolio website.
* Generate production-ready static files.
* Host the website using AWS S3 Static Website Hosting.
* Configure public access using bucket policies.
* Make the website accessible globally through a public URL.

## Technologies Used

* React
* TypeScript
* Vite
* Tailwind CSS
* AWS S3
* AWS IAM
* Static Website Hosting

## Architecture

```text
User Browser
      |
      v
Internet
      |
      v
AWS S3 Bucket
      |
      v
Static Website Files
(HTML, CSS, JavaScript)
```

## Deployment Steps

### Step 1: Build the React Application

```bash
npm install
npm run build
```

This generates a `dist` folder containing static files.

### Step 2: Create an AWS S3 Bucket

* Open AWS Console
* Navigate to Amazon S3
* Create a new bucket
* Disable Block Public Access for the bucket

### Step 3: Upload Website Files

Upload all contents from the generated `dist` folder:

```text
assets/
certificates/
index.html
robots.txt
Midhun_Kumar_Resume.pdf
```

### Step 4: Enable Static Website Hosting

Configure:

```text
Index document: index.html
Error document: index.html
```

### Step 5: Configure Bucket Policy

Allow public read access to website files.

### Step 6: Access Website

Use the S3 Website Endpoint URL to access the live portfolio website.

## Features

* Responsive portfolio website
* About Me section
* Skills section
* Projects section
* Certifications section
* Achievements section
* Resume download option
* Publicly accessible through AWS S3

## Learning Outcomes

* AWS S3 Static Website Hosting
* Cloud Storage Concepts
* Bucket Policies and Public Access
* Static Website Deployment
* Production Build Generation using Vite
* Hosting Frontend Applications without Servers

## Repository Structure

```text
task-1-s3-static-portfolio/
│
├── README.md
├── screenshots/
├── deployment-files/
│   ├── assets/
│   ├── certificates/
│   ├── index.html
│   ├── robots.txt
│   └── Midhun_Kumar_Resume.pdf
```

## Author

**Midhun Kumar V**
