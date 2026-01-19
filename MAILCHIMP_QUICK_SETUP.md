# 🚀 Mailchimp Setup - Step by Step

Follow these exact steps to complete your Mailchimp integration in 5 minutes.

---

## Step 1: Create Your Mailchimp Account

1. Go to **https://mailchimp.com/**
2. Click **Sign Up** (top right)
3. Enter your email address
4. Create a password
5. Check your email for verification link and click it
6. Complete the profile setup

---

## Step 2: Create Your Audience (Mailing List)

1. Log into Mailchimp dashboard
2. Click **Audience** (left sidebar)
3. Click **Create an Audience** (blue button)
4. Fill in the form:
   - **Audience name:** `NilPay Waitlist`
   - **Company name:** `NilPay`
   - **Website:** `https://chap-malok.github.io/nilpay`
   - **Default from name:** `NilPay Team`
   - **Default from email:** Use your email
   - Leave other fields as default
5. Click **Create Audience**

---

## Step 3: Get Your User ID

1. Click your profile icon (top right)
2. Click **Account**
3. Click **Extras** → **API Keys**
4. You'll see your API key like: `a1b2c3d4e5f6g7h8i9j0k1l2-us3`
5. **Copy the part BEFORE the dash** (the long string)
   - Example: `a1b2c3d4e5f6g7h8i9j0k1l2` = YOUR_USER_ID
6. **Note your server prefix** (after the dash)
   - Example: `us3` = YOUR_SERVER (could be us1, us2, us3, etc.)

**Save these values:**
```
YOUR_USER_ID = a1b2c3d4e5f6g7h8i9j0k1l2
YOUR_SERVER = us3
```

---

## Step 4: Get Your List ID

1. Go back to your Audience
2. Click **Audience** (left sidebar) → Select "NilPay Waitlist"
3. Click **Settings** → **Audience name and defaults**
4. Look at the URL in your browser:
   ```
   https://us3.admin.mailchimp.com/lists/[LIST_ID]/settings/list-name
                                            ↑
                                       Copy this
   ```
5. The list ID is the long code in the URL
   - Example: `abcd1e2f3g` = YOUR_LIST_ID

**Save this:**
```
YOUR_LIST_ID = abcd1e2f3g
```

---

## Step 5: Update Your Landing Page

Now you have all three values:
- `YOUR_USER_ID` = a1b2c3d4e5f6g7h8i9j0k1l2
- `YOUR_LIST_ID` = abcd1e2f3g
- `YOUR_SERVER` = us3

**Open `index.html` in VS Code**

Find line ~100 that looks like:
```html
<form class="waitlist-form" action="https://nilpay.us21.list-manage.com/subscribe/post?u=YOUR_USER_ID&amp;id=YOUR_LIST_ID&amp;f_id=YOUR_FORM_ID"
```

Replace it with YOUR actual values:
```html
<form class="waitlist-form" action="https://nilpay.us3.list-manage.com/subscribe/post?u=a1b2c3d4e5f6g7h8i9j0k1l2&amp;id=abcd1e2f3g&amp;f_id=abcd1e2f3g"
```

**Key points:**
- Replace `us21` with your server (us1, us2, us3, etc.)
- Replace `YOUR_USER_ID` with your actual user ID
- Replace `YOUR_LIST_ID` with your actual list ID
- `f_id` is usually the same as `YOUR_LIST_ID`

---

## Step 6: Save and Deploy

1. Save the file (Ctrl + S)
2. Open PowerShell and run:

```powershell
cd "c:\Users\Admin\Desktop\NilPay"
$env:Path = [System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User")
git add .
git commit -m "Add Mailchimp credentials"
git push
```

3. Wait 2-3 minutes for GitHub Pages to update

---

## Step 7: Test Your Form

1. Go to **https://chap-malok.github.io/nilpay**
2. Scroll to the waitlist form
3. Enter a test email
4. Click "Join Waitlist"
5. Go to Mailchimp → **Audience** → **All Contacts**
6. Your test email should appear! ✅

---

## 🎉 Success!

Your form is now live and capturing emails to Mailchimp!

**What happens next:**
- Each person who joins gets added to your audience
- You can send campaigns to them
- You can set up automations (welcome emails, announcements, etc.)

---

## Quick Reference

| Item | Where to Find |
|------|---------------|
| User ID | Account → Extras → API Keys (long string before dash) |
| Server | Account → Extras → API Keys (after dash: us1, us2, us3, etc.) |
| List ID | Your Audience → Settings → Audience name and defaults (in URL) |

---

**Done with Mailchimp setup? I can help with:**
- ✅ Google Analytics
- ✅ Email automations
- ✅ SEO optimization
- ✅ Social media graphics

Let me know what to do next!
