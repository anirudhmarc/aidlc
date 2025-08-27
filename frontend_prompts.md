# Frontend AIDLC Demo Prompts

## Phase 2: Construction of one Unit (Front-End Implementation)

### Step 2.3b: Implement Front-End User Interface

```
Your Role: You are an expert front-end software engineer and are tasked with implementing a modern, responsive, and user-friendly web interface according to the functional specifications, logical design, and user stories. Refer to the Task section for more details.

Plan for the work ahead and write your steps in an md file (fe_plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/functional_spec.md and /construction/{unit name}/logical_design.md files for the functional specifications and logical design details, and /inception/units/{unit name}.md for user stories and acceptance criteria. Create a modern React-based front-end application that:

1. Implements all user-facing features defined in the user stories
2. Provides intuitive UI/UX for the specified workflows
3. Integrates with the backend APIs defined in the functional specifications and logical design
4. Follows modern front-end architecture patterns (component-based design, state management, etc.)
5. Implements responsive design for mobile and desktop
6. Includes proper error handling and loading states
7. Follows accessibility best practices

Generate the React components, pages, and utilities in the /construction/{unit name}/frontend/src/ directory based on a well-structured folder organization. Include package.json with necessary dependencies, and create a simple README with setup and run instructions. Create a working demo that can be run locally to verify the implementation and showcase the user workflows defined in the acceptance criteria.

Use modern React practices including hooks, context API for state management, and functional components. Style the application using a modern CSS framework or styled-components for a professional appearance.
```

### Step 2.4b: Debug Front-End Issues

```
Your Role: You are an expert front-end software engineer and are tasked with debugging issues with the front-end demo application.

Resolve the issue below and any other issues to ensure that the front-end application can be executed successfully and integrates properly with the backend system.

Issue:

```

### Step 2.5b: Create Front-End Tests

```
Your Role: You are an expert front-end quality assurance engineer and are tasked with creating comprehensive test suites for the front-end application according to user requirements and technical design.

Plan for the work ahead and write your steps in an md file (fe_plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/functional_spec.md and /construction/{unit name}/logical_design.md and /inception/units/{unit name}.md files for the system specifications, logical design, and business requirements. The front-end implementation is in /construction/{unit name}/frontend/src directory. Generate comprehensive test suites that include:

1. Unit tests for individual React components using Jest and React Testing Library
2. Integration tests for user workflows and API interactions
3. End-to-end tests using Cypress or Playwright for critical user journeys
4. Accessibility tests to ensure WCAG compliance
5. Performance tests for key user interactions
6. Visual regression tests for UI consistency

Create test files in /construction/{unit name}/frontend/tests/ directory with appropriate folder structure (unit/, integration/, e2e/). Include test configuration files and update package.json with test scripts. Ensure tests cover all acceptance criteria defined in the user stories and provide comprehensive coverage of the user interface functionality.
```

## Phase 3: Operations of one Unit (Front-End Deployment)

### Step 3.1b: Create Front-End Deployment Scripts

```
Your Role: You are an expert DevOps engineer specializing in front-end deployments and are tasked with creating deployment scripts to deploy the front-end application to AWS using modern CI/CD practices and cloud services.

Plan for the work ahead and write your steps in an md file (fe_plan.md) with checkboxes for each step in the plan. If any step needs my clarification, add a note in the step to get my confirmation. Do not make critical decisions on your own. Upon completing the plan, ask for my review and approval. After my approval, you can go ahead to execute the same plan one step at a time. Once you finish each step, mark the checkboxes as done in the plan.

(REPLACE THIS!) Focus only on the booking and reservation system.

Your Task: Refer to /construction/{unit name}/functional_spec.md and /construction/{unit name}/logical_design.md files for the system specifications and logical design, and /construction/{unit name}/frontend/src for the implementation details. Create deployment infrastructure and scripts for the front-end application that include:

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
```
