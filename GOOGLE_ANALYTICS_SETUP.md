# 📊 Google Analytics Setup - Complete Guide

Track who visits your NilPay landing page, where they come from, and how they interact with it.

---

## Step 1: Create Google Analytics Account

1. Go to **https://analytics.google.com/**
2. Click **Start measuring**
3. Enter account name: **NilPay**
4. Click **Next**

---

## Step 2: Create a Property

1. Property name: **NilPay Website**
2. Timezone: **Your timezone** (or UTC)
3. Currency: **USD** (or your preferred)
4. Click **Next**

---

## Step 3: Create a Data Stream

1. Select **Web**
2. **Website URL:** `https://chap-malok.github.io/nilpay`
3. **Stream name:** `NilPay Landing Page`
4. Click **Create stream**

---

## Step 4: Get Your Measurement ID

After creating the stream:
1. You'll see **Measurement ID** (starts with `G-`)
2. Example: `G-ABC123XYZ456`
3. **Copy this ID** - you need it!

---

## Step 5: Add Analytics to Your Site

Google Analytics code has already been added to your `index.html`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-YOUR_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-YOUR_ID');
</script>
```

**You need to replace `G-YOUR_ID` with your actual Measurement ID**

---

## Step 6: Update Your Measurement ID

Ask me to replace `G-YOUR_ID` with your actual ID from Step 4.

Example: If your ID is `G-ABC123XYZ456`, I'll update the code.

Just provide your Measurement ID!

---

## Step 7: Test Analytics

1. After updating your code, wait 1 minute
2. Go to your site: `https://chap-malok.github.io/nilpay`
3. Go back to Google Analytics
4. Click **Realtime** (left menu)
5. You should see yourself visiting! ✅

---

## 📊 What You Can Track

Google Analytics shows you:

### **Audience**
- How many people visit
- Where they're from (country, city)
- What device they use (mobile, desktop, tablet)
- What browser (Chrome, Firefox, Safari)

### **Behavior**
- What pages they visit
- How long they stay
- What they click on
- Scroll depth (how far down they scroll)

### **Conversions** (Advanced)
- Track form submissions
- Track button clicks
- Set goals (e.g., "Join Waitlist")

---

## 🎯 Key Metrics to Monitor

| Metric | What It Means |
|--------|---------------|
| **Sessions** | Number of visits |
| **Users** | Unique people visiting |
| **Bounce Rate** | % who leave without action |
| **Avg. Session Duration** | How long people stay |
| **Pages/Session** | Average pages viewed per visit |

---

## 📈 View Your Analytics

1. Go to **https://analytics.google.com/**
2. Select **NilPay** property
3. Click **Reports** (left menu)
4. Choose what to view:
   - **Overview** - Summary dashboard
   - **Real-time** - Live visitors
   - **Traffic** - Where visitors come from
   - **Engagement** - How they interact

---

## ⏱️ Timeline

- **Immediate:** Code added to your site
- **1-2 hours:** Analytics starts collecting data
- **24 hours:** Full picture visible
- **30 days:** Trends become clear

---

## 🔗 Useful Links

- **View Analytics:** https://analytics.google.com/
- **Google Analytics Help:** https://support.google.com/analytics
- **Measurement ID Location:** Property Settings → Data Streams

---

## Summary

1. ✅ Create Google Analytics account
2. ✅ Create property and data stream
3. ✅ Get Measurement ID (G-...)
4. ✅ Tell me your ID
5. ✅ I'll update your site
6. ✅ Start tracking visitors!

---

**Ready? Give me your Measurement ID and I'll activate analytics on your site!**
