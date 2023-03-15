# Link
http://www.architecturalkatas.com/kata.html?kata=NoBusiness.json

# Description

Client wants to build a toolset/framework/whatever for creating e-business portals for small businesses (customers) to sell to their customers (users)

Requirements: all the usual requirements of an e-commerce package (reliability, user management, money exchange (credit cards, checks, other?), etc); no customer-facing hosting; minimal customer administration; internationalization mandatory

Users: (up to) millions of users per customer, (up to) thousands (or more) of customers


# Users
- Customers
- Users of the customers

# Integrations
- Currency exchange
- payment gateway
- shipping and tracking

# User Interfaces
- Web

# Existing Solutions
There are 2 open source solutions on top of them we can develop these solutions.

- https://smartstore.com/en/tips-tricks-multistores-with-smartstore-one-installation-multiple-shops/
- https://devdocs.magento.com/guides/v2.3/config-guide/multi-site/ms_websites.html

# Technology
- Because of the vast community support, plugin and resource availability Magento is the right choice for this platform
- This solution will require settin up a Store Controller module so that we can setup a new store when a new business sign up

# Infrastrucure
- For a multi tenant approach we need to scale / manage the Store Controller separately
- Through CICD we can setup and deploy a new store on the fly for a new store
- Depending upon the nature / user load different stores can have different independent deployments

# CI/CD
- TBD

# Testing Strategy (Need team to validate and provide input)
- Web Cypress browser based automation to test the application flows
- API Automation using k6 to put load
- Socket IO / realtime load testing?

# Non functional requirements
- High availability (during a disaster should be able to recover data from previous day) with minimal latency say < 300 ms
- The system should be scalable and efficient expected user load 100 concurrent users

# Traffic
- 



