# OTTFLIX

#  OTTFLIX - Netflix Inspired OTT Platform

##  Project Overview

OTTFLIX is a Netflix-inspired OTT platform developed using HTML, CSS, and JavaScript. The application is hosted on an AWS EC2 instance using the Apache web server, while movie posters and trailer videos are stored in an Amazon S3 bucket.

Users can browse movie posters, view a featured banner, and watch movie trailers directly from the website.

---

## Features

- Netflix-inspired user interface
- Responsive design
- Auto-changing banner slider
- Trending movies section
- Watch Trailer popup
- Movie posters stored in Amazon S3
- Trailer videos streamed from Amazon S3
- Hosted on AWS EC2

---

##  Technologies Used

### Frontend
- HTML5
- CSS3
- JavaScript

### AWS Services
- Amazon EC2
- Amazon S3

### Web Server
- Apache2

### Operating System
- Ubuntu

---

## ☁ AWS Architecture

```
User
   │
   ▼
Amazon EC2 (Apache Server)
   │
Loads index.html
   │
   ▼
Amazon S3 Bucket
   ├── Movie Posters
   └── Trailer Videos
``
---

##  How to Run

1. Launch an Ubuntu EC2 instance.
2. Install Apache.

```
sudo apt update
sudo apt install apache2 -y
```

3. Copy the `index.html` file to:

```
/var/www/html/
```

4. Upload movie posters and trailer videos to an Amazon S3 bucket.

5. Replace the poster and trailer URLs in the HTML with your S3 object URLs.

6. Open the website:

```
http://<EC2-Public-IP>
