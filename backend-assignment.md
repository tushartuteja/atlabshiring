---
layout: default
title: Backend Assignment - Atlabs
permalink: /backend-assignment/
---

# Backend Assignment: Video Processing System

## Overview

Build a robust video processing system that demonstrates your backend development skills using Django. The system should handle video file uploads, process them asynchronously, and status updates.

## Core Requirements

### Authentication & Security

- User registration and login
- JWT-based authentication
- Password change functionality that invalidates existing JWTs
- Rate limiting for API endpoints per user
- File upload handling

### Video Processing

- Accept video file uploads (support common formats: MP4, AVI, MOV, WMV, FLV)
- Maximum file size: 500MB
- Generate unique task IDs for each upload
- Process videos using FFmpeg to convert to MP4
- Generate thumbnails for each video
- Implement a queue system that processes one video at a time
- Provide estimated processing time at submission (30 seconds per minute of video)
- Send email notifications upon completion

### Analytics Dashboard for Devops

- Number of files processed
- Time taken to process files (30 seconds per minute of handling)
- Failure rate and failure handling
- Queue length and wait times
- Processing time distribution
- User activity metrics
- System resource utilization

### Technical Requirements

#### Backend (Django)

- Django REST Framework for APIs
- Celery for async task processing
- Redis for:
  - Task queue management
  - Caching task statuses
  - Rate limiting
- FFmpeg for video processing
- JWT authentication
- Email service integration
- Proper error handling and logging

## API Endpoints

### Authentication

- `POST /api/auth/register/` - User registration
- `POST /api/auth/login/` - User login
- `POST /api/auth/change-password/` - Change password
- `POST /api/auth/logout/` - Logout (invalidate JWT)

### Video Processing

- `POST /api/videos/upload/` - Upload video file
- `GET /api/videos/tasks/` - List all tasks
- `GET /api/videos/tasks/{task_id}/` - Get task status
- `GET /api/videos/tasks/{task_id}/thumbnail/` - Get task thumbnail
- `GET /api/videos/tasks/{task_id}/progress/` - Get task progress
- `GET /api/videos/analytics/` - Get processing analytics
- `GET /api/videos/analytics/queue/` - Get queue status
- `GET /api/videos/analytics/system/` - Get system metrics

## Evaluation Criteria

### 1. Code Quality

- Clean, readable, and well-organized code
- Proper error handling
- Comprehensive logging
- Type hints and documentation
- Test coverage

### 2. Architecture & Design

- Scalable system design
- Proper separation of concerns
- Efficient resource utilization
- Security best practices
- API design and documentation

### 3. Feature Implementation

- All core features working as specified
- Proper async task handling
- Efficient state management
- Email notifications
- Thumbnail generation
- Implement progress tracking during processing

### 4. Performance & Reliability

- Proper queue management
- Resource optimization
- Error recovery
- System monitoring

### 5. Security

- Proper authentication
- Rate limiting
- Input validation
- Error message security

## Bonus Points

- Add support for multiple output formats
- Implement video compression options
- Add video metadata extraction
- Implement task prioritization
- Add system health monitoring
- Implement task cancellation

## Submission Guidelines

1. Create a private GitHub repository
2. Add `tushartuteja` as a collaborator
3. Include in your repository:

   - Complete source code
   - Comprehensive README.md with:
     - Setup instructions
     - Architecture decisions
     - API documentation
   - Docker Compose file
   - Environment variables template
   - Test coverage report

4. Send an email to [tushar@atlabs.ai](mailto:tushar@atlabs.ai) with:
   - GitHub repository link
   - Brief overview of your implementation
   - Any challenges faced and how you solved them
   - Time spent on the assignment

## Time Expectation

- Expected time: 1-2 days of Implementation time
- Submission time: 5 days

## Need Help?

If you have any questions or need clarification, please email [tushar@atlabs.ai](mailto:tushar@atlabs.ai)

[Back to Home](/)
