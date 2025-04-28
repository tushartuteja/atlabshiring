---
layout: default
title: Full Stack Assignment - Atlabs
permalink: /fullstack-assignment/
---

# Full Stack Assignment: Collaborative Todo App

## Overview

Build a real-time collaborative Todo application that demonstrates your full-stack development skills using React and Django.

## Core Requirements

### Authentication

- User signup with email verification
- User login/logout
- Password reset functionality

### Task Management

- Create, read, update, and delete task lists
- Add tasks to lists
- Mark tasks as complete/incomplete
- Delete tasks
- Organize tasks within lists (Bonus)

### Collaboration Features

- Share task lists with other users
- Two permission levels:
  - View only
  - Edit access
- Real-time updates using WebSocket (Django Channels)
  - When a task is added/updated/deleted
  - When list permissions change
  - When new users are added to a list

### Technical Requirements

#### Frontend (React)

- Use React with TypeScript
- State management 
- React Router for navigation
- Proper loading states and error handling
- Follow the provided Figma design
- Responsive design (Bonus)

#### Backend (Django)

- Django REST Framework for APIs
- Django Channels for WebSocket
- JWT authentication
- Proper model relationships and database design
- API documentation

## Design

The UI/UX design is available in this [Figma file](https://www.figma.com/design/2MbArFjmOaEjtEbQZXwmY7/To-do-List--Hiring-Assignment?node-id=11-2&t=mIhueILqNzeHmdxT-1). Please follow the design system, components, and interactions specified.

## Deployment

Choose one of the following:

1. Deploy the application (e.g., Heroku, DigitalOcean, AWS)
2. Provide a Docker Compose setup that runs with a single command:

```bash
docker-compose up
```

## Evaluation Criteria

### 1. Code Quality

- Clean, readable, and well-organized code
- Proper component structure in React
- Django best practices and patterns
- Type safety (TypeScript)
- Comments and documentation

### 2. Feature Implementation

- All core features working as specified
- Real-time updates working correctly
- Authentication and authorization
- Error handling and edge cases

### 3. UI/UX Implementation

- Faithful implementation of Figma design
- Responsive design
- Loading states and transitions
- Error states and user feedback

### 4. Technical Choices

- Project structure
- Package choices and implementation
- Performance considerations
- Security best practices

### Bonus Points

- Test coverage (both frontend and backend)
- Additional features that enhance user experience
- Performance optimizations
- Comprehensive documentation

## Using AI Tools

You are encouraged to use AI tools (like GitHub Copilot, ChatGPT) to help with the development. However, please note:

- You should understand every line of code in your submission
- The follow-up interview will involve pair programming to modify and extend your implementation
- Document which AI tools were used and how they helped

## Submission Guidelines

1. Create a private GitHub repository
2. Add `tushartuteja` as a collaborator
3. Include in your repository:

   - Complete source code (frontend and backend)
   - Comprehensive README.md with:
     - Setup instructions
     - Architecture decisions
   - Docker Compose file (if not deployed)
   - Environment variables template

4. Send an email to [tushar@atlabs.ai](mailto:tushar@atlabs.ai) with:
   - GitHub repository link
   - Deployed application link (if applicable)
   - Brief overview of your implementation
   - Any challenges faced and how you solved them
   - Time spent on the assignment

## Time Expectation

- Expected time: 1-2 days
- Maximum time: 4 days

## Need Help?

If you have any questions or need clarification, please email [tushar@atlabs.ai](mailto:tushar@atlabs.ai)

[Back to Home](/)
