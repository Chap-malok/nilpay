# 🎯 Complete Mailchimp Setup for NilPay

Your Mailchimp form is now integrated! Follow these steps to activate it.

## Step 1: Create Mailchimp Account

1. Go to **https://mailchimp.com/**
2. Click **Sign Up** (top right)
3. Create account with your email
4. Complete email verification

## Step 2: Create Your Audience (Mailing List)

1. In dashboard, click **Audience** (left menu)
2. Click **Create Audience**
3. Fill in:
   - **Audience name:** NilPay Waitlist
   - **Company name:** NilPay
   - **Website:** https://chap-malok.github.io/nilpay
   - **Subscriber permission:** Non-profit (free tier)
4. Click **Create Audience**

## Step 3: Get Your Form Credentials

1. Go to **Audience** → **Manage Audience**
2. Click **Signup Forms** → **Signup Forms**
3. In the form settings, find and copy:
   - **Audience ID** (also called List ID)
   - Your account **User ID**

You can find these in the Mailchimp URL when you're in your audience:
```
https://us[X].admin.mailchimp.com/lists/[AUDIENCE_ID]/dashboard
                                    ↑                      ↑
                              YOUR_LIST_ID      From URL above
```

And your User ID from:
1. Account → **Extras** → **API keys**
2. Your User ID is a long number in the API key

## Step 4: Update Your Landing Page

Replace the three placeholders in `index.html`:

**Find this line (around line 100):**
```html
<form class="waitlist-form" action="https://nilpay.us21.list-manage.com/subscribe/post?u=YOUR_USER_ID&amp;id=YOUR_LIST_ID&amp;f_id=YOUR_FORM_ID"
```

**Replace with your actual values:**
```html
<form class="waitlist-form" action="https://nilpay.us[X].list-manage.com/subscribe/post?u=12345678901234567890&amp;id=abcd1e2f3g&amp;f_id=h9i8j7k6l5"
```

Where:
- `us[X]` = Your server prefix (us1, us2, us3, etc.) - find in API key or account settings
- `12345678901234567890` = YOUR_USER_ID
- `abcd1e2f3g` = YOUR_LIST_ID
- `h9i8j7k6l5` = YOUR_FORM_ID (often same as LIST_ID)

## Step 5: Find Your Server Prefix

Easiest way:
1. Go to **Account** → **Extras** → **API keys**
2. Your API key shows format: `[key]-[SERVER_PREFIX]`
3. Example: `a1b2c3d4e5f6g7h8i9j0k1l2-us3`
4. Your server is **us3**

## Step 6: Update and Deploy

1. Open `index.html` in VS Code
2. Find line ~100 with the form action
3. Replace YOUR_USER_ID, YOUR_LIST_ID, YOUR_FORM_ID
4. Save file
5. Run in terminal:
```powershell
cd "c:\Users\Admin\Desktop\NilPay"
git add .
git commit -m "Integrate Mailchimp waitlist form"
git push
```

6. Wait 2-3 minutes for GitHub Pages to update

## Step 7: Test Your Form

1. Go to **https://chap-malok.github.io/nilpay**
2. Enter a test email in the form
3. Click "Join Waitlist"
4. Go to your Mailchimp Audience → **All Contacts**
5. Your email should appear!

## 🎉 You're Done!

Now when people visit your site and join:
- ✅ Their email goes directly to Mailchimp
- ✅ You can see all subscribers in your Audience
- ✅ You can send campaigns to your waitlist
- ✅ You can set up automations (welcome emails, announcements, etc.)

## What's Next?

### Send Welcome Email
1. In Mailchimp: **Automations** → **Create Automation**
2. Choose "Welcome Series"
3. Send a thank you email when someone joins

### Send Announcements
1. **Campaigns** → **Create Campaign**
2. Design email
3. Send to your "NilPay Waitlist" audience

### View Analytics
1. **Audience** → **Dashboard**
2. See subscriber growth, open rates, etc.

## Troubleshooting

**Form not submitting?**
- Make sure you replaced all three placeholders
- Check your Mailchimp settings are correct
- Test in incognito/private browser

**Email not appearing in Mailchimp?**
- Wait 1-2 minutes, refresh
- Check spam folder
- Verify form endpoint is correct

**Can't find credentials?**
- Go to **Account** → **Extras** → **API keys** for User ID
- Go to your audience URL for List ID
- List ID might also be called "Audience ID"

---

**Questions?** Let me know which step you're on and I'll help!
