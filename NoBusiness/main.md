# Link
http://www.architecturalkatas.com/kata.html?kata=NoBusiness.json

# Description

Client wants to build a toolset/framework/whatever for creating e-business portals for small businesses (customers) to sell to their customers (users)

Requirements: all the usual requirements of an e-commerce package (reliability, user management, money exchange (credit cards, checks, other?), etc); no customer-facing hosting; minimal customer administration; internationalization mandatory

Users: (up to) millions of users per customer, (up to) thousands (or more) of customers


# Users
- Sellers
- Buyers

# Integrations


# User Interfaces
- Web
- Mobile

# Technology
- Backend - C#/Java/Node anything that client wants or we have team capacity available
- Database - start with relational database
- Web - Single Page Application (SPA) with mobile responsiveness, ideally ReactJS
- Mobile - React Native cross platform app because the scope doesn't look big and apart from Location no other native functionality mentioned

# Infrastrucure
- Containers / K8 / API Gateway + Labmda functions
- S3 for storage of pictures, frontend assets
- Cloudfront for web deployment
- Testflight for mobile

# CI/CD
- Github actions, upload to container/lambda

# Testing Strategy (Need team to validate and provide input)
- Web Cypress browser based automation to test the application flows
- API Automation using k6 to put load
- Socket IO / realtime load testing?

# Non functional requirements
- High availability (during a disaster should be able to recover data from previous day) with minimal latency say < 300 ms
- The system should be scalable and efficient expected user load 100 concurrent users

# Traffic
- 



