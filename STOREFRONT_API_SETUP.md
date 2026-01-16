# Storefront API Token Setup Guide

## Step 1: Create a Custom App in Shopify Admin

1. **Go to your Shopify Admin**
   - Navigate to: **Settings** → **Apps and sales channels**

2. **Access App Development**
   - Click on **"Develop apps"** (at the bottom of the page)
   - If this is your first time, click **"Allow custom app development"**

3. **Create a New App**
   - Click **"Create an app"**
   - Enter app name: `Size Guide API` (or any name you prefer)
   - Click **"Create app"**

## Step 2: Configure Storefront API Scopes

1. **Configure Storefront API Access**
   - Click on **"Configure Storefront API scopes"**

2. **Select Required Scopes**
   - Check the following scopes:
     - ✅ `unauthenticated_read_product_listings`
     - ✅ `unauthenticated_read_metaobjects` (REQUIRED for size guide)
   
3. **Save Configuration**
   - Click **"Save"** at the top right

## Step 3: Install the App and Get Token

1. **Install the App**
   - Click **"Install app"** button
   - Confirm the installation

2. **Get Your Access Token**
   - Go to **"API credentials"** tab
   - Under **"Storefront API access token"**, you'll see your token
   - Click **"Reveal token once"** or copy the visible token
   - **⚠️ IMPORTANT**: Copy this token immediately - you won't be able to see it again!

## Step 4: Add Token to Your Theme Section

1. **Open Shopify Theme Editor**
   - Go to: **Online Store** → **Themes**
   - Click **"Customize"** on your active theme

2. **Add the Section to a Product Page**
   - Navigate to any product page
   - Click **"Add section"**
   - Search for **"Product Info Size Guide"**
   - Add the section

3. **Configure the Section**
   - Click on the section to open settings
   - Scroll to **"Storefront API Configuration"**
   - Paste your token in the **"Storefront API Access Token"** field
   - Click **"Save"**

## Step 5: Create a Size Guide Metaobject

1. **Go to Metaobjects**
   - Navigate to: **Settings** → **Custom data** → **Metaobjects**

2. **Create Metaobject Definition**
   - Click **"Add definition"**
   - Name: `Size Guide`
   - Type: `size_guide` (must match exactly!)
   - Click **"Add"**

3. **Add Fields to Definition**
   - Add field: **Title**
     - Type: `Single line text`
     - Key: `title`
   - Add field: **Body**
     - Type: `Rich text`
     - Key: `body`
   - Click **"Save"**

4. **Create a Size Guide Entry**
   - Click **"Add entry"**
   - Fill in:
     - **Title**: "Size Guide" (or your preferred title)
     - **Body**: Add your size guide content (tables, text, etc.)
   - Click **"Save"**

## Troubleshooting

### Token Not Working?
- Make sure you copied the entire token (no spaces)
- Verify the `unauthenticated_read_metaobjects` scope is enabled
- Check browser console for error messages

### No Data Showing?
- Verify metaobject type is exactly `size_guide` (lowercase, underscore)
- Make sure you have at least one published metaobject entry
- Check that field keys are `title` and `body` (lowercase)

### CORS Errors?
- This shouldn't happen with Storefront API, but if it does:
  - Make sure you're using the Storefront API token (not Admin API)
  - Check that your shop domain is correct

## Security Notes

✅ **Safe to use in themes:**
- Storefront API tokens are public and read-only
- They're designed to be used in client-side code
- They can only read public data

❌ **NEVER use in themes:**
- Admin API tokens
- Private app passwords
- Any credentials with write access

---

## Quick Reference

**Token Location in Code:**
```liquid
<!-- In section settings -->
"storefront_api_token": "YOUR_TOKEN_HERE"
```

**Metaobject Requirements:**
- Type: `size_guide`
- Fields: `title` (text), `body` (rich text)

**API Scopes Needed:**
- `unauthenticated_read_metaobjects`
