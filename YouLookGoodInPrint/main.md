# Link
[http://www.architecturalkatas.com/kata.html?kata=TakingRequests.json](http://www.architecturalkatas.com/kata.html?kata=YouLookGoodInPrint.json)

# Description

A local copy shop chain wants to offer its customers an "all-in-one" computing experience: document creation, editing, storage and printing

Requirements: browser-based or –delivered; word processing; presentations; document templates (as start points); versioning; print scheduling; automatic and manual payment

Users: initially, thousands in the local city, but potentially millions if the demand grows


# Users
- DJ
- Users

# Integrations

- Music tracks
- Social Login

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
This will be a read-heavy system, so let's assume a 100:1 read/write ratio with 100 million links generated per month.


