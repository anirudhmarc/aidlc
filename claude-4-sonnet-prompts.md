# AIDLC demo prompts

## Phase 1: Inception

### Step 1.1: Create User Stories

```
Your Role: You are an expert product manager and are tasked with creating well defined user stories that becomes the contract for developing the system as mentioned in the Task section below.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!)  Your Task: I would like to build a travel booking web application. In this application, my customers interacts with AI by specifying all their preferences (dates, location, budget, duration, activities). AI understands the preferences and suggests destinations, itineraries and budgets. Once the customer confirms, the system books the flights, hotels and attractions.

Create an /inception/ directory and write the user stories to overview_user_stories.md in the inception directory. Only foucs on user stories and nothing else.
```

### Step 1.2: Grouping User Stories into Units

```
Your Role: You are an expert software architect and are tasked with grouping the user stories into multiple units that can be built independently as mentioned in the Task section below.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

Your Task: Refer to the user stories in, /inception/overview_user_stories.md file. Group the user stories into multiple units that can be built independently. Each unit contains highly cohesive user stories that can be built by a single team. The units must be loosely coupled with each other. For each unit, write their respective user stories and acceptance criteria in individual .md files in the /inception/units/ folder. Do not start the technical systems design yet.
```

## Phase 2: Construction of one Unit

### Step 2.1: Design Domain Model with DDD

```
Your Role: You are an expert software architect and are tasked with designing the domain model using Domain Driven Design for a unit of of the software system. Refer to the Task section for more details.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /inception/units/ folder, each md file represents a software unit with the corresponding user stories. Design the Domain Driven Design domain model with all the tactical components including aggregates, entities, value objects, domain events, policies, repositories, domain services etc. Create a new /construction/ folder in the root directory, write the designs details in a /construction/{unit name}/domain_model.md file.
```

### Step 2.2: Create Logical Design

```
Your Role: You are an expert software architect and are tasked with creating a logical design of a highly scalable, event-driven system according to a Domain Driven Design domain model. Refer to the Task section for more details.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/domain_model.md file for the domain model. Generate a logical design for software source code implementation. Write the design document to the /construction/{unit name}/logical_design.md file. For all /construction/{unit name}/logical_design.md  and /inception/units/{unit name}.md for user stories create a /construction/{unit name}/function_spec that will be used to build a front end 
```

### Step 2.3: Implement Source Code

```
Your Role: You are an expert software engineer and are tasked with implementing a highly scalable, event-driven system according to the Domain Driven Design logical design. Refer to the Task section for more details.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

(!!!REVIEW THIS!!!) Your Task: Refer to /construction/{unit name}/logical_design.md file for the logical design details. Generate a very simple and intuitive python implementation for the bounded context. Assume the repositories and the event stores are in-memory. Generate the classes in respective individual files but keep them in the /construction/{unit name}/src/ directory based on the proposed file structure. Create a simple demo script that can be run locally to verify the implementation.
```

### Step 2.4: Debugging Source Code

```
Your Role: You are an expert software engineer and are tasked with debugging issues with the demo application.

Resolve the issue below and any other issues to ensure that the demo script can be executed successfully.

Issue:

```

Step 2.3b: Implement Front-End User Interface
Your Role: You are an expert front-end software engineer and are tasked with implementing a modern, responsive, and user-friendly web interface according to the Domain Driven Design logical design and user stories. Refer to the Task section for more details.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/logical_design.md file for the logical design details and /inception/units/{unit name}.md for user stories and acceptance criteria. Create a modern React-based front-end application that:

1. Implements all user-facing features defined in the user stories
2. Provides intuitive UI/UX for the domain workflows
3. Integrates with the backend APIs defined in the logical design
4. Follows modern front-end architecture patterns (component-based design, state management, etc.)
5. Implements responsive design for mobile and desktop
6. Includes proper error handling and loading states
7. Follows accessibility best practices

Generate the React components, pages, and utilities in the /construction/{unit name}/frontend/src/ directory based on a well-structured folder organization. Include package.json with necessary dependencies, and create a simple README with setup and run instructions. Create a working demo that can be run locally to verify the implementation and showcase the user workflows defined in the acceptance criteria.

Use modern React practices including hooks, context API for state management, and functional components. Style the application using a modern CSS framework or styled-components for a professional appearance.
Step 2.4b: Debug Front-End Issues
Your Role: You are an expert front-end software engineer and are tasked with debugging issues with the front-end demo application.

Resolve the issue below and any other issues to ensure that the front-end application can be executed successfully and integrates properly with the backend system.

Issue:
Step 2.5b: Create Front-End Tests
Your Role: You are an expert front-end quality assurance engineer and are tasked with creating comprehensive test suites for the front-end application according to user requirements and technical design.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/logical_design.md and /inception/units/{unit name}.md files for the system design and business requirements. The front-end implementation is in /construction/{unit name}/frontend/src directory. Generate comprehensive test suites that include:

1. Unit tests for individual React components using Jest and React Testing Library
2. Integration tests for user workflows and API interactions
3. End-to-end tests using Cypress or Playwright for critical user journeys
4. Accessibility tests to ensure WCAG compliance
5. Performance tests for key user interactions
6. Visual regression tests for UI consistency

Create test files in /construction/{unit name}/frontend/tests/ directory with appropriate folder structure (unit/, integration/, e2e/). Include test configuration files and update package.json with test scripts. Ensure tests cover all acceptance criteria defined in the user stories and provide comprehensive coverage of the user interface functionality.
Phase 3: Operations of one Unit (Front-End Deployment)
Step 3.1b: Create Front-End Deployment Scripts
Your Role: You are an expert DevOps engineer specializing in front-end deployments and are tasked with creating deployment scripts to deploy the front-end application to AWS using modern CI/CD practices and cloud services.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/logical_design.md files for the system design and /construction/{unit name}/frontend/src for the implementation details. Create deployment infrastructure and scripts for the front-end application that include:

1. CloudFormation templates for AWS S3 static website hosting
2. CloudFront distribution for global CDN and HTTPS
3. Route 53 configuration for custom domain (optional)
4. AWS CodePipeline for CI/CD automation
5. Build scripts for optimized production builds
6. Environment-specific configuration management
7. Monitoring and logging setup using CloudWatch

Generate all deployment files in /operations/{unit name}/frontend/ directory including:
- CloudFormation templates (.yaml files)
- Build and deployment scripts
- Environment configuration files
- CI/CD pipeline configuration
- Documentation for deployment process

Ensure the deployment supports multiple environments (dev, staging, production) and includes proper security configurations, caching strategies, and rollback capabilities.


### Step 2.6: Create Tests

```
Your Role: You are an expert quality assurance engineer and are tasked with creating test plans according to the user requirements and technical design for the software systems.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

(REVIEW THIS!) Your Task: Refer to /construction/{unit name}/domain_design.md and /construction/{unit name}/logical_design.md files for the software system design. The implementation is in /construction/{unit name}/src directory if you need more details. Refer to the business requirements for this software unit, including user stories and acceptance criteria in individual .md files in the /inception/units/{unit name}.md file. Generate test plans to test the backend system of this software unit.
```

## Phase 3: Operations of one Unit

### Step 3.1: Create IaC Scripts

```
Your Role: You are an expert devops engineer and are tasked with creating deployment scripts in cloud formation to deploy the selected unit of software to an AWS account based on the specifications of the logical deisgn.

Plan for the work ahead and write your steps in an md file (plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

(REVIEW THIS!) Your Task: Refer to /construction/{unit name}/logical_design.md files for the software system design. The implementation is in /construction/{unit name}/src directory if you need more details. Generate deployment scripts to deploy the backend system of this software unit to AWS in /operation/{unit name}/ directory.
