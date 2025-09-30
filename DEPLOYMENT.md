# CDDT Website Deployment Guide

## Quick Setup Instructions for GitHub Pages

### Prerequisites
- GitHub account
- All website files ready (index.html, css/, js/ folders)

### Step-by-Step Deployment

#### 1. Create Repository
1. Go to GitHub.com and sign in
2. Click "New repository" (green button)
3. Repository name: `cddt-website`
4. Description: "Official website for CDDT - Center for Developing Drone Technologies, RNSIT"
5. Set to **Public**
6. Check "Add a README file"
7. Click "Create repository"

#### 2. Upload Files
Method 1 - Web Interface:
1. Click "uploading an existing file"
2. Drag and drop all files from cddt-website folder
3. Commit message: "Deploy CDDT website"
4. Click "Commit changes"

Method 2 - Git Commands (if you have Git installed):
```bash
git clone https://github.com/YOUR_USERNAME/cddt-website.git
cd cddt-website
# Copy all files to this directory
git add .
git commit -m "Deploy CDDT website"
git push origin main
```

#### 3. Enable GitHub Pages
1. Go to repository Settings tab
2. Click "Pages" in left sidebar
3. Source: "Deploy from a branch"
4. Branch: "main" 
5. Folder: "/ (root)"
6. Click "Save"

#### 4. Access Website
- URL: `https://YOUR_USERNAME.github.io/cddt-website/`
- Wait 5-10 minutes for deployment
- Check the Pages section for deployment status

### Custom Domain Setup (Optional)
If you want to use a custom domain like cddt.rnsit.ac.in:

1. Add a CNAME file to your repository with your domain
2. Configure DNS settings with your domain provider
3. Point your domain to YOUR_USERNAME.github.io
4. Enable HTTPS in repository settings

### Troubleshooting

**Site not loading?**
- Check if all files uploaded correctly
- Ensure index.html is in root directory
- Wait 10-15 minutes for GitHub to build the site

**CSS/JS not working?**
- Verify file paths in index.html are correct
- Check that css/ and js/ folders exist
- Ensure file names match exactly (case-sensitive)

**Want to update the site?**
- Edit files directly on GitHub using the pencil icon
- Or upload new versions of files
- Changes appear within minutes

### File Structure Checklist
```
cddt-website/
├── index.html          ✓ Main website file
├── css/
│   └── style.css       ✓ Styling
├── js/
│   └── script.js       ✓ JavaScript functionality
└── README.md           ✓ Documentation
```

### Contact Integration
The website includes:
- Email links to cddt@rnsit.ac.in
- Contact form (basic HTML form)
- All contact information for CDDT

### Performance Tips
- Website loads fast (no heavy dependencies)
- Mobile-responsive design
- SEO-friendly structure
- Optimized for all devices

---

🚁 **Your CDDT website will be live and accessible worldwide!**

For any deployment issues, contact the technical team or refer to GitHub Pages documentation.
