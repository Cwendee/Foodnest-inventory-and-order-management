# FoodNest Inventory and Order Management

## Overview
FoodNest is a mid-sized e-commerce company specializing in online food sales, offering users a seamless experience managing inventory and tracking orders. The company relies heavily on its CI/CD pipeline to implement updates for its website and mobile applications. The DevOps team uses Jenkins as the primary CI/CD tool, integrating it with GitHub for version control and Maven for managing Java-based microservices. FoodNest frequently rolls out updates to enhance customer experience and introduce new features.

Recently, during a key sales period, FoodNest experienced ongoing failures in its CI/CD pipeline, preventing code from being deployed to production. This caused delays in essential bug fixes and feature updates, adversely affecting the performance and user experience on their e-commerce platform. This project aims to automate these processes for better efficiency and reliability.

Key Issues:

Out-of-Sync Inventory Management

Scenario: Real-time inventory updates are crucial; however, CI/CD pipeline failures resulted in a bug preventing proper synchronization with the backend system.
Impact: Customers may attempt to order out-of-stock items, leading to cancellations and dissatisfaction, or they might be misled about item availability, resulting in lost sales.
Order Tracking Failures

Scenario: The app offers real-time updates on order status. Failures in the CI/CD pipeline disrupted integration with the tracking system, causing users to miss critical updates about their orders.
Impact: This lack of updates can lead to user anxiety and frustration, increase customer service inquiries, and possibly result in order cancellations.

Proposed Solutions:
Enhanced Monitoring: Implement robust monitoring and alerting systems to identify and resolve pipeline failures quickly.

Automated Rollback: Establish automated rollback mechanisms to revert to the last stable version in case of deployment failures.

Comprehensive Testing: Increase the scope and coverage of automated tests, including unit, integration, and end-to-end tests, to catch issues early in the CI/CD process.

Regular Pipeline Reviews: Conduct periodic reviews of the CI/CD pipeline to identify bottlenecks and areas for improvement, ensuring that integrations with third-party services are resilient.

Documentation and Training: Maintain thorough documentation and provide ongoing training for the DevOps team to improve troubleshooting capabilities and efficiency in managing the CI/CD pipeline.

As part of the review process and to address the issues encountered with the FoodNest app, I executed automation tests using Maven builds to identify the root causes of the CI/CD pipeline failures. These tests allowed for a thorough analysis of the existing codebase, helping to pinpoint specific errors that were contributing to the deployment issues.

Additionally, I conducted further testing within Jenkins to validate the effectiveness of the proposed corrections. This iterative approach ensured that the fixes were implemented and tested thoroughly within the CI/CD environment, paving the way for a more stable deployment process.

By leveraging both Maven and Jenkins for automated testing, we were able to enhance the reliability of the CI/CD pipeline, ensuring smoother future updates and an improved user experience on the FoodNest platform.


## Features
- Real-time inventory management
- Order tracking and status updates
- Automated build and deployment using Jenkins and Maven

## Technologies Used
- **Java**: Core programming language
- **Spring Boot**: Framework for building the application
- **Maven**: Dependency management and build automation
- **Jenkins**: CI/CD for continuous integration and deployment

## Getting Started
### Prerequisites
- Java 17 or higher
- Maven
- Git

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Cwendee/Foodnest-inventory-and-order-management
