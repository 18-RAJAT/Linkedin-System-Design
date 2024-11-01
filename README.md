# Professional Networking Platform (LinkedInConnect)

A scalable and secure cloud-based networking platform inspired by LinkedIn, designed to facilitate professional connections, job search, and member engagement. This platform supports job postings, company pages, groups, content creation, messaging, and more, enabling professionals to connect, share content, and engage with each other. Deployed on AWS and Vercel, and powered by a React frontend, this platform integrates a variety of AWS services and databases optimized for both social connections and job search capabilities.

## Table of Contents

1. [Overview](#overview)
2. [Architecture](#architecture)
   - [Authentication](#authentication)
   - [Profile Management](#profile-management)
   - [Search Capabilities](#search-capabilities)
   - [Connection Requests](#connection-requests)
   - [Recommendations](#recommendations)
   - [Profile Statistics](#profile-statistics)
   - [Content Creation and Engagement](#content-creation-and-engagement)
   - [Messaging and Notifications](#messaging-and-notifications)
   - [Company Pages and Job Listings](#company-pages-and-job-listings)
   - [Groups](#groups)
   - [Following](#following)
   - [Payment and Subscription](#payment-and-subscription)
3. [Frontend and Deployment](#frontend-and-deployment)
4. [Database Design](#database-design)
   - [Graph Database](#graph-database)
   - [SQL Database](#sql-database)
5. [Cloud Infrastructure on AWS](#cloud-infrastructure-on-aws)

---

## 1. Overview

This platform is built for professionals to connect, engage, and search for job opportunities while managing and showcasing their profiles. Key features include member profiles, content creation, messaging, notifications, job postings, and more.

## 2. Architecture

### Authentication
- Users can authenticate using GitHub or email.

### Profile Management
- Members can create and manage profiles, including details like basic info, work experiences, education, skills, and accomplishments.

### Search Capabilities
- A robust search function allows users to find other members or companies by name.

### Connection Requests
- Members can send and accept connection requests, helping them build their professional network.

### Recommendations
- Users can request and receive recommendations from other members.

### Profile Statistics
- Statistics like profile views, connections, and search appearances are displayed on each member profile.

### Content Creation and Engagement
- Members can create posts, comment, like, or share content with their connections.

### Messaging and Notifications
- Direct messaging is available, with notifications for new messages, connection invitations, and comments on posts.

### Company Pages and Job Listings
- Companies can create pages and post job listings.

### Groups
- Members can create or join groups to connect with like-minded individuals.

### Following
- Members can follow other members or companies for updates.

### Payment and Subscription
- Payments for subscriptions are enabled using Stripe and card payments.

## 3. Frontend and Deployment
- The frontend is built with React and deployed on Vercel for optimal performance and scalability.

## 4. Database Design

### Graph Database
- A graph database is used to store user activities, connections, and relationships.

### SQL Database
- A SQL database is utilized for storing job listings and related data.

## 5. Cloud Infrastructure on AWS
- **AWS EC2**: Used for hosting backend services with scalable configurations.
- **AWS S3**: Stores user profile images, post media, and other assets.
- **AWS Lambda**: Manages serverless functions for handling notifications and other asynchronous tasks.
- **AWS RDS**: Hosts the SQL database for job listings.
- **AWS Neptune**: Manages the graph database for efficient handling of user connections and relationships.
- **AWS SNS/SQS**: Used for messaging queues and notifications, ensuring real-time updates for user activities.
- **AWS Cognito**: Provides secure authentication with GitHub and email support.
