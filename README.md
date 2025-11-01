# Onurix API - Postman Collection

[![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)](https://www.postman.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

![Onurix Logo](https://cdn.onurix.com/web/assets/img/logo50.png)

This repository contains the official Postman collection for the **Onurix API**. Use this collection to easily test and integrate Onurix services including SMS, Voice Calls, WhatsApp, URL Shortener, and contact management into your applications.

## 📋 Table of Contents

- [Features](#-features)
- [Getting Started](#-getting-started)
- [Installation](#-installation)
- [Configuration](#-configuration)
- [Collection Structure](#-collection-structure)
- [Usage Examples](#-usage-examples)
- [API Documentation](#-api-documentation)
- [Support](#-support)
- [License](#-license)

## ✨ Features

This Postman collection includes all major Onurix API endpoints:

- **SMS**: Send text messages and 2FA codes
- **Voice Calls**: Generate automated voice calls with custom messages
- **WhatsApp**: Send WhatsApp messages with templates and 2FA codes
- **General**: Check balance, verify messages, manage security
- **Groups & Contacts**: Complete contact and group management
- **URL Shortener**: Create and track shortened URLs

## 🚀 Getting Started

### Prerequisites

- [Postman](https://www.postman.com/downloads/) installed (Desktop App or Web Version)
- An active Onurix account
- Your API credentials (Client ID and API Key)

### Get Your API Credentials

1. Log in to your [Onurix panel](https://onurix.com)
2. Navigate to **Seguridad API** (API Security)
3. Copy your **Client ID** and **API Key**

## 📥 Installation

### Method 1: Import from File

1. Download the collection file: `Onurix-API.postman_collection.json`
2. Open Postman
3. Click **Import** button (top left)
4. Drag and drop the JSON file or click **Upload Files**
5. Click **Import**

### Method 2: Import from GitHub

1. Open Postman
2. Click **Import** button
3. Select **Link** tab
4. Paste the raw GitHub URL of the collection file:
   ```
   https://raw.githubusercontent.com/onurixlatam/postman/main/Onurix-API.postman_collection.json
   ```
5. Click **Continue** and then **Import**

## ⚙️ Configuration

After importing the collection, you need to configure your API credentials:

### Option 1: Using Environment Variables (Recommended)

1. In Postman, click on **Environments** (left sidebar)
2. Click **Create Environment** (or use an existing one)
3. Add the following variables:
   - `client` = Your Client ID from Onurix panel
   - `key` = Your API Key from Onurix panel
4. Click **Save**
5. Select the environment from the dropdown in the top-right corner

### Option 2: Using Collection Variables

1. Right-click on the **Onurix API** collection
2. Select **Edit**
3. Go to the **Variables** tab
4. Update the values for:
   - `client` = Your Client ID
   - `key` = Your API Key
5. Click **Save**

## 📂 Collection Structure

The collection is organized into the following folders:

### 1. SMS
- **Send SMS**: Send text messages to one or multiple recipients
- **Send SMS 2FA**: Send SMS with two-factor authentication codes

### 2. Calls
- **Send Call**: Generate voice calls with custom messages
- **Send Call 2FA**: Send 2FA codes via voice call

### 3. WhatsApp
- **Send WhatsApp with Template**: Send messages using approved Meta templates
- **Send WhatsApp 2FA**: Send 2FA codes via WhatsApp
- **Send WhatsApp Without Template**: Send direct messages

### 4. General
- **Get Balance**: Check your account credit balance
- **Security - Block Number**: Block phone numbers
- **Verify 2FA Code**: Validate two-factor authentication codes
- **Verify Message Status**: Check delivery status of messages

### 5. Groups and Contacts
- **Create/Update/Delete Groups**: Manage contact groups
- **Create/Update/Delete Contacts**: Manage individual contacts
- **List Groups**: View all contact groups
- **List Contacts in Group**: View contacts in a specific group
- **Associate/Dissociate Contacts**: Manage group memberships

### 6. URL Shortener
- **Create Short URL**: Generate shortened URLs
- **Get URL Statistics**: Track clicks and analytics for shortened URLs

## 💡 Usage Examples

### Example 1: Send an SMS

1. Open the **SMS** folder
2. Click on **Send SMS**
3. Make sure your environment is selected
4. Update the request body parameters:
   - `phone`: Replace with destination number (e.g., `573001234567`)
   - `sms`: Enter your message text
5. Click **Send**

### Example 2: Check Your Balance

1. Open the **General** folder
2. Click on **Get Balance**
3. Click **Send**
4. View your credit balance in the response

### Example 3: Create a Contact Group

1. Open the **Groups and Contacts** folder
2. Click on **Create Group**
3. Update the `name` parameter in the request body
4. Click **Send**
5. Note the `group-id` in the response for future use

### Example 4: Send WhatsApp Message

1. Open the **WhatsApp** folder
2. Click on **Send WhatsApp with Template**
3. Update the URL query parameter `templateId` with your approved template ID
4. Modify the JSON body with your data:
   - `phones`: Destination number(s)
   - `header`, `body`, `button`: Template parameter values
5. Click **Send**

## 📚 API Documentation

For detailed API documentation, including:
- Complete parameter descriptions
- Response formats and status codes
- Rate limits and best practices
- Advanced usage scenarios

Please visit the official documentation: [https://docs.onurix.com/](https://docs.onurix.com/)

## 🔗 Related Resources

- [Onurix cURL Examples](https://github.com/onurixlatam/onurix-curl) - Command-line examples
- [Onurix PHP SDK](https://github.com/onurixlatam/onurix-php) - PHP integration
- [Onurix Python SDK](https://github.com/onurixlatam/onurix-python) - Python integration
- [Onurix Node.js SDK](https://github.com/onurixlatam/onurix-nodejs) - Node.js integration
- [Onurix Java SDK](https://github.com/onurixlatam/onurix-java) - Java integration
- [Onurix Go SDK](https://github.com/onurixlatam/onurix-go) - Go integration
- [Onurix C# SDK](https://github.com/onurixlatam/onurix-csharp) - C# integration

## 🔐 Security Notes

- **Never commit your API credentials** to version control
- Store your `client` and `key` values in Postman environments
- Use environment-specific credentials (development, staging, production)
- Rotate your API keys periodically from the Onurix panel

## 📞 Support

For support and questions:

- **Email**: soporte@onurix.com
- **Website**: [https://onurix.com](https://onurix.com)
- **Documentation**: [https://docs.onurix.com/](https://docs.onurix.com/)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

---

Made with ❤️ by [Onurix](https://onurix.com)