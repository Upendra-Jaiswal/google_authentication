# google_authentication
# Google Authentication Project

## Overview

This project demonstrates how to implement Google Authentication in a web application using the Google Cloud Platform (GCP). With Google Authentication, users can easily sign in to your application using their Google credentials.

## Setup

1. Go to [Google Cloud Platform](https://console.cloud.google.com/) and create a new project.

2. Navigate to "APIs & Services" > "Credentials" in the GCP Console.

3. Click on "Create Credentials" and select "OAuth client ID."

4. Choose "Web application" as the application type.

5. Enter your application's name and authorized JavaScript origins (e.g., `http://localhost:3000` for local development).

6. Add "Authorized redirect URIs" (e.g., `http://localhost:3000/auth/google/callback`).

7. Click "Create" to generate your client ID and secret key.

## Environment Variables

Create a `.env` file in the root directory of your project and add the following environment variables:

```plaintext
GOOGLE_CLIENT_ID=your_client_id_here
GOOGLE_CLIENT_SECRET=your_client_secret_here
```

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/your_username/google-auth-project.git
   cd google-auth-project
   ```

2. Install the required dependencies using yarn:
   ```
   yarn install
   ```

## Running the Project

1. Start the development server:
   ```
   npm start
   ```

2. Open your web application at `http://localhost:3000` and test the Google Authentication.

## Dependencies

- Express.js: Backend server
- Passport.js: Authentication middleware
- Passport-google-oauth20: Google OAuth 2.0 strategy for Passport.js
- dotenv: For loading environment variables from `.env` file

## Contributing

Contributions are welcome! If you have any improvements or bug fixes, feel free to submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
