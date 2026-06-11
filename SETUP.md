# GitHub Pages Setup Instructions

This repository is configured for automatic deployment to GitHub Pages using GitHub Actions.

## 🚀 Quick Setup

Follow these steps to enable your academic CV website:

### 1. Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/ferhatalkan/FerhatAlkan`
2. Click on **Settings** (in the repository menu)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - **Source**: GitHub Actions
5. Click **Save**

### 2. Merge Your Branch to Main

The GitHub Actions workflow is configured to deploy from the `main` branch. You need to merge your feature branch:

```bash
git checkout main
git merge claude/check-scholar-access-JOGRy
git push origin main
```

Or create a Pull Request on GitHub and merge it.

### 3. Wait for Deployment

- Once you push to `main`, GitHub Actions will automatically build and deploy your site
- Go to the **Actions** tab in your repository to watch the deployment progress
- Deployment typically takes 1-2 minutes

### 4. Access Your Site

Your academic CV will be available at:
```
https://ferhatalkan.github.io/FerhatAlkan/
```

## 📁 Files Added

This setup includes:

- **`.github/workflows/pages.yml`** - GitHub Actions workflow for automatic deployment
- **`.nojekyll`** - Tells GitHub Pages not to process files with Jekyll
- **`index.html`** - Your main academic CV page
- **`404.html`** - Custom error page
- **`CNAME`** - Optional custom domain configuration (currently commented out)

## 🌐 Custom Domain (Optional)

If you want to use a custom domain:

1. Purchase a domain from a registrar
2. Uncomment and edit the `CNAME` file with your domain
3. Configure DNS settings at your registrar:
   - For apex domain (yourdomain.com): Add A records pointing to GitHub Pages IPs
   - For subdomain (www.yourdomain.com): Add CNAME record pointing to `ferhatalkan.github.io`
4. Enable "Enforce HTTPS" in GitHub Pages settings

GitHub Pages IPs (for A records):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

## 🔄 Updating Your CV

Whenever you want to update your CV:

1. Edit `index.html` or `README.md`
2. Commit your changes
3. Push to `main` branch
4. GitHub Actions will automatically redeploy your site

## 📝 What's Included

Your academic CV includes:

- ✅ Research background and contributions
- ✅ Publication list with descriptions
- ✅ Research expertise areas
- ✅ Education history
- ✅ Technical skills
- ✅ Professional contact information
- ✅ Links to Google Scholar, ORCID, ResearchGate
- ✅ Responsive mobile-friendly design
- ✅ SEO optimization
- ✅ Social media sharing meta tags

## 🎨 Customization

You can customize the CV by editing `index.html`:

- **Colors**: Modify the gradient colors in the CSS
- **Content**: Update any section content
- **Styling**: Adjust fonts, spacing, layouts
- **Add sections**: Add new research areas, publications, or skills

## 🐛 Troubleshooting

**Site not deploying?**
- Check the Actions tab for error messages
- Ensure GitHub Pages is enabled in settings
- Verify you pushed to the `main` branch

**404 errors?**
- GitHub Pages can take a few minutes to propagate
- Clear your browser cache
- Check that the file names are correct (case-sensitive)

**Need help?**
- Check GitHub Pages documentation: https://docs.github.com/en/pages
- View workflow runs in the Actions tab

## 📞 Support

For questions or issues with the academic CV setup, check:
- GitHub Pages Status: https://www.githubstatus.com/
- GitHub Pages Documentation: https://docs.github.com/en/pages

---

**Your academic CV is ready to go live!** 🎉

Once you complete the setup steps above, your research profile will be accessible to the world at:
**https://ferhatalkan.github.io/FerhatAlkan/**
