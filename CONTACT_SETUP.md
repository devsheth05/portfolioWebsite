# Contact Form Setup Guide

Your portfolio website now has a contact form, but it needs to be configured to actually send emails. Here are your options:

## Option 1: EmailJS (Recommended - Free)

EmailJS is a service that lets you send emails directly from JavaScript without a backend server.

### Setup Steps:

1. **Sign up for EmailJS**:
   - Go to [emailjs.com](https://www.emailjs.com/)
   - Create a free account
   - You get 200 emails per month for free

2. **Add your email service**:
   - Go to Email Services in your dashboard
   - Click "Add New Service"
   - Choose your email provider (Gmail, Outlook, etc.)
   - Follow the setup instructions

3. **Create an email template**:
   - Go to Email Templates
   - Click "Create New Template"
   - Use this template:

```html
Subject: New message from {{from_name}} - {{subject}}

Name: {{from_name}}
Email: {{from_email}}
Subject: {{subject}}

Message:
{{message}}
```

4. **Get your credentials**:
   - Service ID: Found in Email Services
   - Template ID: Found in Email Templates  
   - Public Key: Found in Account > API Keys

5. **Update the JavaScript**:
   In `script.js`, replace these placeholders:
   ```javascript
   emailjs.init('YOUR_PUBLIC_KEY'); // Line 47
   emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', templateParams) // Line 67
   to_name: 'Your Name' // Line 60
   ```

## Option 2: Simple Mailto Link (Easiest)

This opens the user's default email client with a pre-filled message.

### Setup:
1. In `script.js`, find the `setupMailtoFallback()` function
2. Replace `your.email@example.com` with your actual email
3. Uncomment the function call at the bottom of the file

## Option 3: Netlify Forms (If using Netlify)

If you deploy to Netlify, you can use their built-in form handling.

### Setup:
1. Add `netlify` attribute to your form:
   ```html
   <form class="contact-form" netlify>
   ```

2. Deploy to Netlify
3. Forms will be handled automatically
4. You'll receive emails at your registered email address

## Option 4: Formspree (Alternative to EmailJS)

Formspree is another popular form handling service.

### Setup:
1. Go to [formspree.io](https://formspree.io/)
2. Create a free account
3. Create a new form
4. Update your HTML form:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

## Quick Test Setup (Mailto)

For now, you can quickly test by using the mailto option:

1. Open `script.js`
2. Find line 47: `emailjs.init('YOUR_PUBLIC_KEY');`
3. Comment out the EmailJS code (lines 44-70)
4. Uncomment the mailto fallback by adding this line at the bottom:
   ```javascript
   setupMailtoFallback();
   ```

## Which Option Should You Choose?

- **EmailJS**: Best for a professional setup, works great
- **Mailto**: Simplest, opens user's email client
- **Netlify Forms**: Perfect if you're using Netlify for hosting
- **Formspree**: Good alternative to EmailJS

## Need Help?

If you get stuck with any of these options, let me know and I can help you set it up step by step! 