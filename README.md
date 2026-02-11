# Kanbanix Board Frontend

Kanbanix Board Frontend is a microfrontend responsible for board and column management.

It is independently deployable and integrated into the Kanbanix Shell using Webpack Module Federation.

## Features

- Create, update, delete boards
- Create and manage columns
- Drag and drop task movement
- Real time board updates
- API integration with Board Service and Task Service

## Architecture

Built with:

- React
- Webpack Module Federation
- React DnD or similar drag and drop library
- REST API integration

## AWS Deployment (Always Free Tier)

Frontend is deployed using:

- Amazon S3 for static hosting
- Amazon CloudFront for CDN delivery
- GitHub Actions for CI/CD pipeline

Each deployment publishes build artifacts to S3 and invalidates CloudFront cache.

## Integration

Loaded dynamically by:

- kanbanix-shell-frontend

This ensures independent scaling and deployment.
