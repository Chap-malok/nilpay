# 🔍 Finding Your Mailchimp Credentials - Visual Guide

Follow these exact steps with screenshots descriptions.

---

## ✅ Step 1: Log Into Mailchimp

1. Go to **https://mailchimp.com/**
2. Click **Sign In** (top right)
3. Enter your email and password
4. Click **Sign In**

---

## ✅ Step 2: Find Your USER ID & SERVER

This is in your **API Key**.

### Go to Account Settings:
1. Click your **profile icon** (top right corner)
2. Click **Account**
3. In the left menu, click **Extras** 
4. Click **API Keys**

### You'll see your API Key:
It looks like this:
```
a1b2c3d4e5f6g7h8i9j0k1l2-us3
↑ This part = USER ID
                        ↑ This part = SERVER
```

**ACTION:**
- Copy everything **BEFORE the dash** = YOUR_USER_ID
- Note everything **AFTER the dash** = YOUR_SERVER

Example:
- User ID: `a1b2c3d4e5f6g7h8i9j0k1l2`
- Server: `us3`

---

## ✅ Step 3: Find Your LIST ID

This is in your **Audience Settings**.

### Go to Your Audience:
1. Click **Audience** (left menu)
2. Select **"NilPay Waitlist"** from the dropdown
3. Click **Settings** (left menu under your audience name)
4. Click **Audience name and defaults**

### Look at Your Browser URL:
The URL will look like:
```
https://us3.admin.mailchimp.com/lists/abcd1e2f3g/settings/list-name
                                        ↑
                                   Copy this = LIST ID
```

**ACTION:**
- Copy the code between `/lists/` and `/settings`
- That's your LIST ID

Example: `abcd1e2f3g`

---

## 📋 Summary - What You Need

Fill in these three values:

```
YOUR_USER_ID = [long string from API key, before dash]
YOUR_SERVER = [after the dash in API key, like us1, us2, us3]
YOUR_LIST_ID = [from your audience URL, between /lists/ and /settings]
```

---

## 🎯 Still Can't Find Them?

Try these alternative methods:

### Method 1: Check Your Email
Mailchimp sends a setup email with your account details. Check your email inbox for "Welcome to Mailchimp".

### Method 2: Create a New Audience
If you can't find your existing audience:
1. Click **Audience** → **Create an Audience**
2. Name it "NilPay Waitlist"
3. Create it
4. Then follow Step 3 above to get the LIST ID

### Method 3: Contact Mailchimp Support
1. Go to **Help** (bottom left in Mailchimp)
2. Click **Contact Us**
3. They can provide your User ID

---

## ⚡ Quick Checklist

- [ ] I found my **USER ID** (long string before dash in API key)
- [ ] I found my **SERVER** (us1, us2, us3, etc. - after dash in API key)
- [ ] I found my **LIST ID** (from audience URL between /lists/ and /settings)

---

## Next Step

Once you have all three values, just tell me:
- YOUR_USER_ID = ?
- YOUR_SERVER = ?
- YOUR_LIST_ID = ?

And I'll update your form immediately! 🚀

---

## Example (Real Values - Don't Use These!)

If you had:
- User ID: `abc123def456`
- Server: `us2`
- List ID: `xyz789`

Your form URL would be:
```
https://nilpay.us2.list-manage.com/subscribe/post?u=abc123def456&id=xyz789&f_id=xyz789
```

---

**Still stuck? Reply with a screenshot or the exact steps you're taking, and I'll help!**
