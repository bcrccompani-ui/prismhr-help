# How to Get Bing to Index Your PrismHR GitHub Pages Site

## What's been done (already updated in the files)
- ✅ sitemap.xml — fixed to use absolute URLs (`https://bcrccompani-ui.github.io/prismhr-help/payroll.html` etc.)
- ✅ robots.txt — fixed to point to the absolute sitemap URL
- ✅ index.html — better SEO meta tags, descriptions, and link titles
- ✅ llms.txt — created (helps AI tools discover content)

## What you need to do

### Step 1: Upload the updated files to GitHub
Go to your repository at **https://github.com/bcrccompani-ui/prismhr-help** and upload these updated files:
- `sitemap.xml`
- `robots.txt`
- `index.html`
- `llms.txt`

### Step 2: Submit to Bing Webmaster Tools (most important step)

1. Go to **https://www.bing.com/webmasters/**
2. Sign in with your **Microsoft work account** (the same one you use for M365)
3. Click **"Add a site"** and enter: `https://bcrccompani-ui.github.io/prismhr-help/`
4. **Verify ownership** — choose the **"HTML meta tag"** method:
   - Bing will give you a meta tag that looks like:
     `<meta name="msvalidate.01" content="XXXXXXXXXXXX">`
   - You need to add that line to the `<head>` section of your `index.html` file
   - I've left a comment in `index.html` showing exactly where to paste it
   - Upload the updated `index.html` to GitHub
   - Click "Verify" in Bing Webmaster Tools
5. After verification, go to **Sitemaps** in the left menu
6. Enter: `https://bcrccompani-ui.github.io/prismhr-help/sitemap.xml`
7. Click **Submit**
8. Go to **URL Inspection** in the left menu
9. Enter `https://bcrccompani-ui.github.io/prismhr-help/` and click **Request Indexing**
10. Also request indexing for key pages like `payroll.html`, `benefits.html`

### Step 3: Wait
- Bing typically takes **24-72 hours** to crawl after submission
- After 3 days, check by searching: `site:bcrccompani-ui.github.io/prismhr-help`
- If results show up, your Copilot agent knowledge source should start working

### Step 4: Test your Copilot agent
Once Bing shows results, go back to your agent and ask a PrismHR question. It should now be able to pull content from the website.