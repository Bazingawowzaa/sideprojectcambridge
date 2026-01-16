# Side Project Network Website

A clean, modern website for the Side Project Network society at the University of Cambridge.

## Quick Start

### Option 1: View Locally
Simply open `index.html` in your browser to preview the site.

```bash
cd /Users/mengqi/Documents/Actions/06-Society/website
open index.html
```

### Option 2: Deploy to GitHub Pages (Free)

1. Create a GitHub repository:
   - Go to github.com and create a new repository
   - Name it `sideprojectcambridge.github.io` (or any name)

2. Push the code:
   ```bash
   cd /Users/mengqi/Documents/Actions/06-Society/website
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/sideprojectcambridge.github.io.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to repository Settings > Pages
   - Source: Deploy from branch
   - Branch: main, / (root)
   - Save

4. Your site will be live at: `https://YOUR_USERNAME.github.io/sideprojectcambridge.github.io`

### Option 3: Deploy to Netlify (Free, Easiest)

1. Go to [netlify.com](https://netlify.com) and sign up
2. Click "Add new site" > "Deploy manually"
3. Drag and drop the entire `website` folder
4. Done! You'll get a URL like `random-name.netlify.app`
5. You can set a custom subdomain like `sideprojectcambridge.netlify.app`

### Option 4: Deploy to Vercel (Free)

1. Go to [vercel.com](https://vercel.com) and sign up
2. Click "Add New Project"
3. Import from GitHub or upload directly
4. Done!

## Customization

### Update Event Details
Edit `index.html`, find the Events section (~line 150), and update:
- Event date
- Event time
- Event location

### Update Google Form Link
Find this line in `index.html`:
```html
<a href="https://forms.gle/YOUR_FORM_ID_HERE" ...>
```
Replace `YOUR_FORM_ID_HERE` with your actual Google Form link.

### Update Social Links
In the footer section, update:
- Instagram URL
- Email address

### Change Colors
Edit `styles.css` and modify the CSS variables at the top:
```css
:root {
    --color-primary: #2D5BFF;      /* Main blue */
    --color-primary-dark: #1E3FAD;  /* Darker blue */
    --color-accent: #FF6B35;        /* Orange accent */
    /* ... */
}
```

### Add Your Photos
Replace the founder initials with actual photos:
1. Add photos to the website folder
2. Replace the `.founder-avatar` divs with `<img>` tags

## File Structure

```
website/
├── index.html      # Main HTML file
├── styles.css      # All styling
└── README.md       # This file
```

## Features

- Fully responsive (mobile, tablet, desktop)
- Modern, clean design
- Smooth scroll navigation
- No JavaScript framework required
- Fast loading
- SEO-friendly

## Custom Domain (Optional)

If you want a custom domain like `sideprojectcambridge.com`:

1. Buy a domain (~£10/year from Namecheap, Google Domains, etc.)
2. In your hosting platform (Netlify/Vercel/GitHub Pages):
   - Add the custom domain in settings
   - Update DNS records as instructed
3. SSL certificate is usually automatic and free

## Need Help?

Contact: sideprojectcambridge@gmail.com
