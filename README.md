# Usertour Examples Repository

This repository contains various examples and deployment configurations for [Usertour](https://usertour.io), a user onboarding and product tour platform.

## Overview

This repository serves as a collection of examples, configurations, and deployment templates for Usertour implementations. It includes ready-to-use configurations for different deployment scenarios and environments.

## Contents

### Docker Compose Configuration for Coolify

The `docker-compose.coolify.yml` file provides a complete Docker Compose configuration optimized for deployment on [Coolify](https://coolify.io), a self-hosted platform-as-a-service solution.

#### Features

- **Complete Stack**: Includes Usertour application, PostgreSQL database, and Redis cache
- **Production Ready**: Configured with production environment variables
- **Easy Deployment**: One-command deployment with Docker Compose
- **Scalable**: Designed for containerized environments

#### Services Included

- **Usertour App**: Main application running on port 8011
- **PostgreSQL**: Database for storing application data
- **Redis**: Cache and session storage

#### Configuration Options

The configuration supports various authentication methods:
- Email authentication (enabled by default)
- GitHub OAuth integration
- Google OAuth integration

Additional features:
- AWS S3 integration for file storage
- Stripe payment processing
- Email service configuration
- JWT token management

## Quick Start

### Deploy with Coolify

1. Clone this repository
2. Use the `docker-compose.coolify.yml` file in your Coolify project
3. Configure the environment variables as needed
4. Deploy the stack

### Local Development

```bash
# Clone the repository
git clone <repository-url>

# Navigate to the project directory
cd examples

# Deploy with Docker Compose
docker-compose -f docker-compose.coolify.yml up -d
```

## Environment Variables

The configuration includes comprehensive environment variable setup for:

- Database connections
- Authentication providers
- File storage (AWS S3)
- Payment processing (Stripe)
- Email services
- Security settings

## Contributing

Feel free to contribute additional examples, configurations, or improvements to this repository. This helps the community by providing more deployment options and use cases.

## License

This repository is provided as-is for educational and deployment purposes.

## Support

For support with Usertour, visit the [official documentation](https://docs.usertour.io) or contact the Usertour team.