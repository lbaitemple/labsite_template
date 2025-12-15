# Quick Start Guide

Get your lab website up and running in 5 minutes!

## Step 1: Install (2 minutes)

```bash
# Install Ruby and Bundler (if not already installed)
gem install bundler

# Install dependencies
cd template
bundle install
```

## Step 2: Configure (1 minute)

Edit `_config.yml`:
```yaml
title: Your Lab Name
email: your-email@university.edu
description: Your lab description
url: "https://yourusername.github.io"
baseurl: "/your-repo-name"  # or "" for root domain
```

## Step 3: Add Content (2 minutes)

### Add Your PI Info
Edit `_pages/team/pi-name.md` with your information

### Add a Student
Copy `_pages/team/phd-student.md` and customize

### Add a Research Project
Copy `_pages/research/sample-project.md` and customize

### Add News
Edit `_data/news.yml` to add news items

### Add Publications
Edit `_data/publications.json` to add papers

## Step 4: Add Images

Place images in:
- `images/team/` - Team photos
- `images/slider/` - Homepage slider (any images here will auto-load)
- `images/research/` - Project images
- `images/news/` - News images

## Step 5: Run Locally

```bash
bundle exec jekyll serve
```

Visit: http://localhost:4000

## Step 6: Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/your-repo.git
git push -u origin main
```

Then enable GitHub Pages in your repository settings!

## What's Included

✅ Responsive design  
✅ Team page with alumni organization  
✅ Research projects with search & filters  
✅ Publications with tabs (Conference/Journal/Year/Search)  
✅ News feed with images  
✅ Dynamic homepage slider  
✅ Mobile-friendly  

## Need Help?

- See `SETUP.md` for detailed instructions
- See `README.md` for full documentation
- Check Jekyll docs: https://jekyllrb.com/docs/

## Customization Tips

- **Colors**: Edit `css/main.scss`
- **Navigation**: Edit `_includes/header.html`
- **Footer**: Edit `_includes/footer.html`
- **Homepage**: Edit `_pages/home.md`

That's it! You're ready to go! 🚀
