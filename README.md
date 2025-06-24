# SWIFTYWAY---RIDER-BOOKING-WEB-APP
# 🚖 Swiftway – Cloud-Native Rider Booking Application

**Swiftway** is a cloud-native rider booking application built with AWS services and modern web technologies. This app allows users to seamlessly book rides, manage their profiles, and access ride details in a secure and scalable environment.

---

## 🌟 Features

- **🔐 User Authentication**: Managed via AWS Cognito for secure sign-up, login, and session management.  
- **🚗 Rider Booking System**: Users can book, view, and manage their rides.  
- **⚙️ Scalable Backend**: Built using AWS Lambda, providing a serverless architecture.  
- **🗂️ Database Management**: Stores ride and user data securely using DynamoDB.  
- **🔁 Continuous Deployment**: Utilizes AWS Amplify with GitHub integration for CI/CD.  
- **📩 Seamless Interaction**: Uses Amazon SNS to send notifications to users through e-mail.

---

## 🛠️ Built With

- **Frontend**:  
  - HTML  
  - CSS  
  - JavaScript

- **Backend Services**:
  - [AWS Amplify](https://aws.amazon.com/amplify/) – Hosting and CI/CD  
  - [AWS Cognito](https://aws.amazon.com/cognito/) – User authentication  
  - [AWS Lambda](https://aws.amazon.com/lambda/) – Serverless backend functions  
  - [AWS IAM](https://aws.amazon.com/iam/) – Access management  
  - [Amazon DynamoDB](https://aws.amazon.com/dynamodb/) – NoSQL database for user and booking data  
  - [Amazon SNS](https://aws.amazon.com/sns/) – User interaction via email  
  - [GitHub](https://github.com) – Version control and deployment

---

## 🚀 Getting Started

### ✅ Prerequisites

- AWS Account (to use AWS services)
- Git (for version control)
- Node.js *(optional for local development)*

### 🧰 Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/swiftway.git
   cd swiftway
---

## ⚙️ Set Up AWS Services

1. **Create a Cognito User Pool**  
   - Go to AWS Cognito in the AWS console.  
   - Create a new User Pool.  
   - Configure an app client (disable client secret if using JavaScript).  
   - Enable necessary authentication flows (e.g., USER_PASSWORD_AUTH).  

2. **Set Up DynamoDB**  
   - Create a new table named `Rides` or `Bookings` with `UserID` or `RideID` as the partition key.  
   - Optionally, create a `Users` table for profile data.

3. **Create AWS Lambda Functions**  
   - Implement logic for booking rides, retrieving user data, and updating bookings.  
   - Connect Lambda with DynamoDB using AWS SDK.

4. **Set Up IAM Roles**  
   - Create custom roles with policies that allow access to Cognito, DynamoDB, and Lambda.  
   - Attach these roles to Amplify and Lambda functions.

---

## 🚀 Configure Amplify

1. **Connect to GitHub**  
   - In AWS Amplify, choose "Host Web App" and connect your GitHub repository.

2. **Configure Backend**  
   - Add Amplify environment variables to access Cognito pool IDs, table names, and API endpoints.  
   - Link Amplify to your Cognito, DynamoDB, and Lambda resources.  
   - Set up CI/CD from your GitHub repo.

---

## 💻 Run the Application

- **Local Testing**:  
  Simply open `index.html` in your browser.

- **Cloud Deployment**:  
  Once deployed via Amplify, you will receive a hosted URL to access your application online.

---

## 🔧 Usage

- **Register / Login**  
  Create an account using the signup page, then log in securely using Cognito authentication.

- **Book a Ride**  
  Use the booking form to select options and submit ride details.

- **View Bookings**  
  Access your dashboard to view, manage, or cancel your bookings.

---

## 🤝 Contributing

We welcome contributions! To contribute:

1. Fork this repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request and describe your changes.

Thank you for helping improve Swiftway!

