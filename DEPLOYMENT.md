# Deployment Guide - The Conscious Project Website

This guide provides step-by-step instructions for deploying The Conscious Project website to various hosting platforms.

## Prerequisites

- All project files (`index.html`, `styles.css`, `script.js`, `README.md`)
- A web hosting account or platform account
- Basic knowledge of file uploads

## Deployment Options

### 1. GitHub Pages (Recommended - Free)

**Steps:**
1. Create a new GitHub repository named `conscious-project-website`
2. Upload all project files to the repository
3. Go to repository Settings
4. Scroll down to "Pages" section
5. Under "Source", select "Deploy from a branch"
6. Choose "main" branch and "/ (root)" folder
7. Click "Save"
8. Your site will be available at: `https://yourusername.github.io/conscious-project-website`

**Custom Domain (Optional):**
1. In Pages settings, add your custom domain
2. Update DNS records with your domain provider
3. Enable HTTPS in Pages settings

### 2. Netlify (Free & Easy)

**Method A - Drag & Drop:**
1. Go to [netlify.com](https://netlify.com)
2. Sign up/login with GitHub, GitLab, or email
3. Drag your project folder to the deploy area
4. Your site is live instantly with a random URL
5. Click "Site settings" to customize the URL

**Method B - Git Integration:**
1. Connect your GitHub repository to Netlify
2. Netlify will auto-deploy on every push
3. Set up custom domain in Site settings

### 3. Vercel (Free)

**Steps:**
1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub, GitLab, or email
3. Click "New Project"
4. Import your repository or drag files
5. Deploy with default settings
6. Customize domain in Project settings

### 4. Traditional Web Hosting

**Steps:**
1. Log into your hosting control panel (cPanel, Plesk, etc.)
2. Navigate to File Manager
3. Go to `public_html` folder (or your domain's root folder)
4. Upload all project files
5. Ensure `index.html` is in the root directory
6. Your site will be accessible via your domain

### 5. Firebase Hosting (Free)

**Steps:**
1. Install Firebase CLI: `npm install -g firebase-tools`
2. Login: `firebase login`
3. Initialize: `firebase init hosting`
4. Select your project folder
5. Deploy: `firebase deploy`

## File Structure for Deployment

Ensure your deployment includes these files:
```
/
├── index.html          # Main page
├── styles.css          # Styles
├── script.js           # JavaScript
├── README.md           # Documentation
├── package.json        # Project info
└── .gitignore          # Git ignore rules
```

## Post-Deployment Checklist

- [ ] Website loads correctly
- [ ] All sections are visible
- [ ] Navigation works properly
- [ ] Responsive design works on mobile
- [ ] All links function correctly
- [ ] Images and graphics display properly
- [ ] No console errors in browser developer tools

## Custom Domain Setup

### For GitHub Pages:
1. Add `CNAME` file with your domain name
2. Update DNS A records to point to GitHub Pages IPs:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153

### For Netlify:
1. Add custom domain in Site settings
2. Update DNS records as instructed by Netlify
3. Enable HTTPS certificate

### For Vercel:
1. Add domain in Project settings
2. Update DNS records as shown in Vercel dashboard
3. SSL certificate is automatic

## Performance Optimization

### Before Deployment:
- [ ] Minify CSS and JavaScript (optional)
- [ ] Optimize images (if any are added)
- [ ] Test loading speed with PageSpeed Insights

### After Deployment:
- [ ] Enable gzip compression (usually automatic)
- [ ] Set up CDN if needed
- [ ] Monitor with Google Analytics (optional)

## SSL/HTTPS Setup

Most modern hosting platforms provide free SSL certificates:
- **GitHub Pages**: Automatic HTTPS
- **Netlify**: Automatic HTTPS
- **Vercel**: Automatic HTTPS
- **Traditional Hosting**: Enable through cPanel or contact support

## Troubleshooting

### Common Issues:

**404 Error:**
- Ensure `index.html` is in the root directory
- Check file permissions
- Verify file names are correct (case-sensitive)

**Styling Issues:**
- Check that `styles.css` is uploaded
- Verify CSS file path in HTML
- Clear browser cache

**JavaScript Not Working:**
- Check browser console for errors
- Ensure `script.js` is uploaded
- Verify JavaScript file path in HTML

**Mobile Issues:**
- Test responsive design
- Check viewport meta tag
- Verify CSS media queries

## Maintenance

### Regular Updates:
- Monitor website performance
- Update content as needed
- Keep dependencies updated
- Backup files regularly

### Security:
- Keep hosting account secure
- Use strong passwords
- Enable two-factor authentication
- Regular security updates

## Support

If you encounter issues:
1. Check the browser console for errors
2. Verify all files are uploaded correctly
3. Test in different browsers
4. Contact your hosting provider's support

---

**Need Help?** Check the main README.md file for additional information and customization options.
