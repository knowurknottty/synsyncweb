# SEO Setup Guide for SynSync Pro

This document contains instructions for completing your SEO setup and submitting to Google Search Console.

## ✅ Completed SEO Tasks

### 1. Title Tags
All pages now have optimized title tags:
- **index.html**: "SynSync Pro — The Linux of Brain Technology"
- **quickref.html**: "SynSync Pro — Quick Reference Card"
- **usermanual.html**: "SynSync Pro — Complete User Manual"

### 2. Meta Descriptions
All pages now have compelling meta descriptions (150-160 characters):
- **index.html**: "Access peer-reviewed neurobiological protocols to restore sleep, dopamine, focus, and emotional balance. 81 protocols. 100+ citations. Your brain, your rules."
- **quickref.html**: "Quick reference guide for all 81 SynSync Pro protocols. Searchable index of neurobiological interventions for sleep, dopamine, focus, and emotional balance."
- **usermanual.html**: "Complete documentation for SynSync Pro. Learn how to use evidence-based neurobiological protocols to optimize sleep, dopamine, focus, and cognitive performance."

### 3. robots.txt
Created at `/robots.txt` with:
- Allows all search engines
- References sitemap.xml
- Includes common bot configurations

**⚠️ ACTION REQUIRED**: Update the sitemap URL in `robots.txt` with your actual domain.

### 4. sitemap.xml
Created at `/sitemap.xml` with all three pages:
- Homepage (priority: 1.0)
- Quick Reference (priority: 0.8)
- User Manual (priority: 0.8)

**⚠️ ACTION REQUIRED**: Update all URLs in `sitemap.xml` with your actual domain.

---

## 📋 Next Steps: Google Search Console Submission

### Step 1: Update Domain URLs
Before submitting, replace `yourdomain.com` in these files with your actual domain:
1. `robots.txt` - Line 6: Sitemap URL
2. `sitemap.xml` - Lines 6, 12, 18: All page URLs

### Step 2: Deploy Your Site
Make sure all files are deployed to your web server:
- index.html
- quickref.html
- usermanual.html
- robots.txt
- sitemap.xml

### Step 3: Verify Domain Ownership in Google Search Console

1. **Go to Google Search Console**
   - Visit: https://search.google.com/search-console

2. **Add Your Property**
   - Click "Add Property"
   - Choose "URL prefix" method
   - Enter your full domain (e.g., `https://yourdomain.com`)

3. **Verify Ownership** (Choose one method):

   **Option A: HTML File Upload (Recommended)**
   - Download the verification file from Google
   - Upload it to your website root
   - Click "Verify"

   **Option B: HTML Tag**
   - Copy the meta tag provided by Google
   - Add it to the `<head>` section of index.html (after the existing meta tags)
   - Deploy the change
   - Click "Verify"

   **Option C: DNS Record**
   - Add a TXT record to your domain's DNS settings
   - Wait for propagation (can take up to 48 hours)
   - Click "Verify"

### Step 4: Submit Your Sitemap

1. In Google Search Console, go to **Sitemaps** (left sidebar)
2. Enter `sitemap.xml` in the "Add a new sitemap" field
3. Click **Submit**
4. Google will begin crawling your site

### Step 5: Monitor Indexing

- Check the **Coverage** report to see which pages are indexed
- Use **URL Inspection** tool to check individual pages
- It typically takes 3-7 days for initial indexing
- Full indexing may take 2-4 weeks

---

## 🎯 SEO Quick Wins (Optional but Recommended)

### Add Open Graph Tags
For better social media sharing, add these to each page's `<head>`:

```html
<!-- Open Graph / Facebook -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://yourdomain.com/">
<meta property="og:title" content="SynSync Pro — The Linux of Brain Technology">
<meta property="og:description" content="Access peer-reviewed neurobiological protocols to restore sleep, dopamine, focus, and emotional balance.">
<meta property="og:image" content="https://yourdomain.com/og-image.jpg">

<!-- Twitter -->
<meta property="twitter:card" content="summary_large_image">
<meta property="twitter:url" content="https://yourdomain.com/">
<meta property="twitter:title" content="SynSync Pro — The Linux of Brain Technology">
<meta property="twitter:description" content="Access peer-reviewed neurobiological protocols to restore sleep, dopamine, focus, and emotional balance.">
<meta property="twitter:image" content="https://yourdomain.com/og-image.jpg">
```

### Add Canonical URLs
Add to each page to prevent duplicate content issues:

```html
<link rel="canonical" href="https://yourdomain.com/">
```

### Schema.org Structured Data
Consider adding JSON-LD structured data for better rich snippets:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebSite",
  "name": "SynSync Pro",
  "url": "https://yourdomain.com",
  "description": "Access peer-reviewed neurobiological protocols to restore sleep, dopamine, focus, and emotional balance."
}
</script>
```

---

## 📊 Tracking Your SEO Progress

### Week 1
- ✅ Site verified in Google Search Console
- ✅ Sitemap submitted
- Check: URL Inspection shows pages are discoverable

### Week 2-3
- Check: Pages begin appearing in Coverage report
- Monitor: Any crawl errors or issues
- Action: Fix any errors reported

### Week 4+
- Check: Pages indexed and appearing in search
- Monitor: Search performance metrics
- Optimize: Based on search query data

---

## 🔧 Troubleshooting

**Pages not being indexed?**
- Check robots.txt isn't blocking pages
- Verify sitemap.xml URLs are correct
- Use URL Inspection tool in Search Console
- Request indexing manually for priority pages

**Sitemap errors?**
- Ensure all URLs use HTTPS (if applicable)
- Check that all URLs return 200 status codes
- Validate sitemap at: https://www.xml-sitemaps.com/validate-xml-sitemap.html

**Need help?**
- Google Search Console Help: https://support.google.com/webmasters
- Sitemap Protocol: https://www.sitemaps.org/protocol.html

---

*Last updated: February 15, 2026*
