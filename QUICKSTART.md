# Quick Start Guide

Get started with the Onurix API Postman Collection in 5 minutes!

## Step 1: Import the Collection

1. Open Postman
2. Click **Import** (top left corner)
3. Select the `Onurix-API.postman_collection.json` file
4. Click **Import**

## Step 2: Import the Environment (Optional)

1. Click **Import** again
2. Select the `Onurix-API.postman_environment.json` file
3. Click **Import**

## Step 3: Configure Your Credentials

### If you imported the environment:
1. Click on **Environments** in the left sidebar
2. Select **Onurix API Environment**
3. Update these values:
   - `client`: Your Client ID from Onurix panel
   - `key`: Your API Key from Onurix panel
4. Click **Save**
5. Select the environment from the dropdown (top right)

### If you didn't import the environment:
1. Right-click on **Onurix API** collection
2. Select **Edit**
3. Go to **Variables** tab
4. Update the `client` and `key` values
5. Click **Save**

## Step 4: Test Your First Request

Let's check your account balance:

1. Expand the **Onurix API** collection
2. Open the **General** folder
3. Click on **Get Balance**
4. Click **Send** button
5. You should see your credit balance in the response!

## Step 5: Send Your First SMS

1. Open the **SMS** folder
2. Click on **Send SMS**
3. In the request body, update:
   - `phone`: Your test phone number (e.g., `573001234567`)
   - `sms`: Your message text
4. Click **Send**
5. Check your phone for the SMS!

## Common Phone Number Format

- **Colombia**: 573001234567
- **Mexico**: 525512345678
- **Argentina**: 541112345678
- **Chile**: 56912345678
- **Peru**: 51912345678

Always use international format (country code + number, no + sign).

## What's Next?

- Explore other endpoints in the collection
- Read the [full README](README.md) for detailed documentation
- Visit [docs.onurix.com](https://docs.onurix.com/) for API reference
- Check out our [SDKs](https://github.com/onurixlatam) for your programming language

## Need Help?

- **Email**: soporte@onurix.com
- **Website**: [onurix.com](https://onurix.com)

## Troubleshooting

### Issue: "Unauthorized" error
**Solution**: Check that your `client` and `key` variables are correctly set with valid credentials.

### Issue: "Invalid phone number" error
**Solution**: Ensure phone numbers are in international format without the + sign (e.g., 573001234567).

### Issue: Environment variables not working
**Solution**: Make sure you've selected the environment from the dropdown in the top-right corner of Postman.

---

Happy testing! 🚀
