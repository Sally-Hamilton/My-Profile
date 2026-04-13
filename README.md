# Instructional Design Portfolio - Setup Guide

## 📋 Overview

This is your professional instructional design portfolio foundation. It includes:
- **Main portfolio page** (`index.html`) - Showcases your work and expertise
- **Project template** (`projects/project-template.html`) - Reusable template for case studies
- Fully responsive design that works on mobile, tablet, and desktop
- Print-friendly for PDF export
- Professional styling ready to customize with your content

## 🎨 What You Have

### Main Portfolio Page (`index.html`)
Your homepage includes these sections:
1. **Hero Section** - Your name, title, and call-to-action
2. **About Section** - Your bio and expertise areas
3. **Featured Projects** - 5 project cards linking to detailed case studies
4. **Skills & Tools** - Your technical skills and methodologies
5. **Process Section** - Your instructional design approach
6. **Contact Section** - Email, LinkedIn, and resume download

### Project Template (`projects/project-template.html`)
A comprehensive case study template with:
- Project overview and context
- Challenge/problem statement
- Your solution and approach
- Learning objectives
- Project details (audience, tools, deliverables)
- Development process
- Key features and interactions
- Results and impact

## 🚀 Getting Started

### Step 1: Customize Your Main Portfolio Page

Open `index.html` and replace all the **yellow highlighted** text with your information:

**Essential Updates:**
1. **Line 7**: Change page title to your name
2. **Line 168**: Replace "Your Name" with your actual name
3. **Line 204-209**: Update your bio paragraphs
4. **Lines 265-338**: Update the 5 project cards:
   - Project titles
   - Descriptions
   - Project types (e-learning, ILT, etc.)
5. **Lines 411-413**: Add your skills and tools
6. **Line 496**: Update your email address
7. **Line 552**: Add your name to footer

**Optional Customizations:**
- **Colors**: Lines 33-55 define the color scheme (change CSS variables in `:root`)
- **Hero tagline**: Line 169 - customize your professional tagline
- **Process steps**: Lines 465-484 - adjust to match your methodology
- **Skills**: Lines 383-448 - add/remove skills relevant to you

### Step 2: Create Your Project Case Studies

For each project you want to showcase:

1. **Duplicate the template**:
   - Copy `projects/project-template.html`
   - Rename it (e.g., `projects/elearning-sales-training.html`)

2. **Fill in your content**:
   - Replace all **yellow highlighted** text with your project details
   - Add real screenshots where you see image placeholders
   - Remove sections that don't apply to your project

3. **Link from main page**:
   - Update the project card link in `index.html` to point to your new file
   - Example: Change `href="projects/project1.html"` to `href="projects/elearning-sales-training.html"`

4. **Repeat for each project** (aim for 3-5 strong examples)

### Step 3: Add Your Project Images

1. Create a folder: `portfolio/images/`
2. Add your screenshots and project images there
3. Reference them in your project pages:
   ```html
   <!-- Replace the image placeholder with: -->
   <img src="../images/your-screenshot.jpg" 
        alt="Description of screenshot" 
        style="width: 100%; border-radius: 0.75rem; box-shadow: var(--shadow);">
   ```

### Step 4: Test Your Changes

1. **Open in browser**: Double-click `index.html` to preview
2. **Check mobile view**: Resize browser window to see responsive design
3. **Test navigation**: Click all links to ensure they work
4. **Review project pages**: Make sure all your case studies look complete

## 📱 Responsive Design

Your portfolio automatically adjusts for:
- **Desktop** (large screens)
- **Tablet** (medium screens)
- **Mobile** (small screens)
- **Print** (generates clean PDFs)

Test by resizing your browser window!

## 🎯 Tips for Strong Project Case Studies

### What Makes a Great Case Study?

1. **Clear Problem Statement**
   - What challenge did you solve?
   - Why did it matter to the organization?

2. **Your Process**
   - Show your instructional design methodology
   - Explain your design decisions
   - Include storyboards or wireframes if available

3. **Measurable Results**
   - Quantitative data (completion rates, test scores, performance improvements)
   - Qualitative feedback (learner testimonials, stakeholder quotes)
   - Business impact (time saved, errors reduced, sales increased)

4. **Visual Examples**
   - Screenshots of key screens
   - Before/after comparisons
   - Sample interactions or assessments
   - Storyboard excerpts

5. **Reflection**
   - What did you learn?
   - What would you do differently?
   - Shows growth mindset and professionalism

### Project Selection

Choose projects that demonstrate:
- **Variety**: Different modalities (e-learning, ILT, job aids, video)
- **Complexity**: Mix of simple and sophisticated projects
- **Impact**: Projects with measurable results
- **Recent work**: Focus on last 2-3 years if possible
- **Your best work**: Quality over quantity - 3-5 strong examples beats 10 mediocre ones

## 🌐 Hosting Options

Once your portfolio is ready, host it online:

### Free Options:
1. **GitHub Pages** (Recommended)
   - Free hosting
   - Custom domain support
   - Version control
   - Tutorial: https://pages.github.com/

2. **Netlify**
   - Free tier with custom domain
   - Drag-and-drop deployment
   - Automatic HTTPS
   - Website: https://www.netlify.com/

3. **Vercel**
   - Free for personal projects
   - Fast deployment
   - Website: https://vercel.com/

### Steps to Deploy:
1. Create account on chosen platform
2. Upload your `portfolio` folder
3. Configure custom domain (optional)
4. Share your portfolio URL!

## 🎨 Customization Tips

### Change Color Scheme

Edit the CSS variables in `index.html` (lines 33-55):

```css
:root {
  --accent: #2563eb;        /* Primary color */
  --accent-hover: #1d4ed8;  /* Hover state */
  --accent-light: #dbeafe;  /* Light accent */
}
```

Popular color schemes for ID portfolios:
- **Professional Blue**: `#2563eb` (current)
- **Creative Purple**: `#7c3aed`
- **Modern Teal**: `#0891b2`
- **Trustworthy Navy**: `#1e40af`

### Add Google Fonts

Add to `<head>` section:
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
```

Update font-family:
```css
body {
  font-family: 'Inter', system-ui, sans-serif;
}
```

### Add Your Logo

Replace the text logo with an image:
```html
<a href="#" class="nav-logo">
  <img src="images/logo.png" alt="Your Name" style="height: 32px;">
</a>
```

## 📄 Export to PDF

To create a PDF version:
1. Open `index.html` in Chrome or Edge
2. Press `Ctrl+P` (Windows) or `Cmd+P` (Mac)
3. Select "Save as PDF"
4. Choose "Background graphics" option
5. Save as `YourName-Portfolio.pdf`

The styling automatically adjusts for clean, professional PDF output!

## ✅ Final Checklist

Before sharing your portfolio:

- [ ] All yellow markers replaced with your content
- [ ] Your name and contact info updated
- [ ] All 5 project cards customized
- [ ] At least 3 detailed project case studies completed
- [ ] Screenshot images added to project pages
- [ ] All links tested and working
- [ ] Viewed on mobile/tablet/desktop (responsive)
- [ ] Spell-checked all content
- [ ] PDF export looks professional
- [ ] Hosted online (if needed for applications)

## 🤝 Need Help?

Common issues and solutions:

**Q: Images aren't showing up**
A: Make sure image paths are correct. Use relative paths like `../images/screenshot.jpg` from project pages.

**Q: Links to project pages are broken**
A: Check that filenames match exactly (including `.html` extension) and that files are in the `projects/` folder.

**Q: Mobile view looks weird**
A: The design is fully responsive. Try resizing your browser or viewing on an actual mobile device.

**Q: Want to add more project cards?**
A: Copy one of the existing project card HTML blocks (lines 265-290) and paste it within the projects-grid div.

## 🎓 Portfolio Best Practices

1. **Keep it updated**: Add new projects as you complete them
2. **Get feedback**: Ask colleagues or mentors to review
3. **Track results**: If projects have measurable impact, add that data
4. **Stay professional**: Proofread carefully, use consistent formatting
5. **Tell your story**: Let your personality and design philosophy shine through

## 📧 Questions?

If you need to customize something not covered here, look for the comments in the HTML code that start with `<!-- === `. These mark the major sections you can modify.

---

**Good luck with your instructional design job search!** This portfolio foundation will help you stand out and showcase your skills effectively.