

# Swiftway - Rider Booking Web App

Swiftway is a cloud-native rider booking application built with AWS services and modern web technologies. This app allows users to seamlessly book rides, manage their profiles, and access ride details in a secure and scalable environment.

## Features

- **User Authentication**: Managed via AWS Cognito for secure sign-up, login, and session management.
- **Rider Booking System**: Users can book, view, and manage their rides.
- **Scalable Backend**: Built using AWS Lambda, providing a serverless architecture.
- **Database Management**: Stores ride and user data securely using DynamoDB.
- **Continuous Deployment**: Utilizes AWS Amplify with GitHub integration for CI/CD.
- **Seamless Interaction**: Uses Amazon SNS to give notifications to the users through e-mail.

## Built With

- **Frontend**: HTML, CSS, JavaScript
- **Backend Services**:
  - AWS Amplify - Hosting and CI/CD
  - AWS Cognito - User authentication
  - AWS Lambda - Serverless backend functions
  - AWS IAM - Access management
  - DynamoDB - NoSQL database for user and booking data
  - GitHub - Version control and deployment
  - Amazon SNS - Interaction with user

## Getting Started

To run Swiftway locally or deploy it to the cloud, follow these steps:

### Prerequisites

- **AWS Account**: Set up an AWS account to use the required services.
- **Git**: Version control for cloning and managing the repository.
- **Node.js** (optional for local development)

### Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/swiftway.git
   cd swiftway
   ```

2. **Install Dependencies** (if applicable):
   ```bash
   npm install
   ```

3. **Set Up AWS Services**:
   - Create a Cognito User Pool and configure the app client for user authentication.
   - Set up DynamoDB to manage user and booking data.
   - Use Lambda for backend logic, such as booking and data management functions.
   - Set up IAM roles to control access to resources.

4. **Configure Amplify**:
   - Connect the repository to AWS Amplify for automated deployments.
   - Configure your environment variables and connect Amplify with Cognito and DynamoDB.

5. **Run the Application**:
   - For local testing, open `index.html` in a web browser.
   - For cloud deployment, Amplify will provide the app URL.


## Usage

- **Register / Login**: Create an account and log in to access booking features.
- **Book a Ride**: Select available options to book a ride.
- **View Bookings**: Manage your bookings through the user dashboard.

## Contributing

We welcome contributions! Please fork the repository and submit a pull request for review.
