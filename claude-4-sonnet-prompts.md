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


### Step 2.5: Create Tests

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
