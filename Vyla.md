# Vyla

A new Flutter project for tracking expenses and managing finances.

## Privacy Policy

**Effective Date:** January 6, 2026

### 1. Introduction
Welcome to **Vyla**. Your privacy is critically important to us. This Privacy Policy explains what information we collect, how we use it, and the choices you have regarding your data when you use our mobile application.

### 2. Information We Collect

#### 2.1 SMS Data (Automated Expense Tracking)
Our application requests permission to **Read SMS messages (`READ_SMS`)**.
- **Purpose:** We use this permission exclusively to identify transaction alerts from banks and financial institutions.
- **Process:** The app scans your SMS inbox locally on your device to extract transaction details such as the amount, merchant name, and date.
- **Privacy:** **We do not upload your SMS messages to any external server.** All parsing and processing logic is executed locally on your device using regular expressions.

#### 2.2 Financial Data
We collect and store the financial data you generate within the app, including:
- Income and expense records.
- Budget limits and financial goals.
- Account names and balances.

#### 2.3 Device Information
We may collect basic device information (e.g., device model, operating system version) to ensure application stability and compatibility.

### 3. How We Use Your Information
We use the information we collect to:
- Automatically categorize expenses based on SMS alerts.
- Provide detailed analytics and charts regarding your spending habits.
- Display your current financial health and budget status.
- Secure specific app features using biometric authentication.

### 4. Data Storage and Security

#### 4.1 Local Storage
- All your transaction history, budgets, and settings are stored locally on your device using **SQLite** databases.
- We do not maintain a central cloud database of your personal financial records.

#### 4.2 Sensitive Data
- Sensitive information, such as user-defined PINs or authentication tokens, is stored securely using **Flutter Secure Storage**, which leverages the Android Keystore and iOS Keychain for encryption.
- We do not store your biometric data. We rely on the local operating system's authentication result (e.g., FaceID, Fingerprint) via the `local_auth` package.

### 5. Third-Party Services

#### 5.1 Google Generative AI
- The application integrates with Google's Generative AI to provide advanced insights or categorization features.
- When you use AI-powered features, specific, anonymized data snippets (e.g., transaction descriptions) may be processed by Google's API to return intelligent responses.
- We do not share your entire SMS inbox or personal identifiers with this service.
- For more information, please review the [Google Privacy Policy](https://policies.google.com/privacy).

### 6. Permissions

To function correctly, the app app requires the following permissions:
- **SMS:** To detect and log transactions automatically.
- **Notification:** To send you alerts when a new transaction is logged or a budget is exceeded.
- **Biometrics:** To enable secure unlock features.
- **Background Service:** To monitor for new SMS messages even when the app is closed.

### 7. Data Deletion
Since all data is stored locally, you can delete all your data by simply uninstalling the application or clearing the app data in your device settings.

### 8. Changes to This Policy
We may update this Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page or within the app updates.

### 9. Contact Us
If you have any questions about this Privacy Policy, please contact us.
