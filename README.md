# Jeba Tasnia - Academic Portfolio

A minimalist, responsive academic portfolio website built with HTML, CSS, and vanilla JavaScript.

## Color Palette
- **Deep Teal:** `#142D2B` (primary accents, navigation)
- **Ivory:** `#F5F3EE` (background, card backgrounds)
- **Muted Gold:** `#B49A78` (accent highlights, hover states)
- **Charcoal:** `#30343B` (body text, headings)
- **White:** `#FFFFFF` (cards, sections)

## Directory Structure
```
portfolio/
├── index.html
├── style.css
├── script.js
├── assets/
│   ├── images/
│   │   └── profile-photo.jpg   (replace with your photo)
│   └── pdfs/
│       └── cv.pdf              (replace with your CV)
│       └── certificate-1.pdf   (replace with your certificates)
│       └── certificate-2.pdf
│       └── certificate-3.pdf
└── README.md
```

## Setup Instructions

### 1. Replace Profile Photo
- Replace `assets/images/profile-photo.jpg` with your actual photo
- Recommended size: 200x200px minimum
- Supported formats: JPG, PNG, WebP

### 2. Replace CV
- Replace `assets/pdfs/cv.pdf` with your actual CV PDF
- The download link is in the Hero section and CV section

### 3. Replace Certificates
- Replace `assets/pdfs/certificate-1.pdf`, `certificate-2.pdf`, `certificate-3.pdf` with your actual certificate PDFs
- Update the certificate links in the Certificates section (modify the HTML to add/remove certificates)

### 4. Update Personal Information
Edit `index.html` and replace the following placeholder text:

**Hero Section:**
- Name: Already set to "Jeba Tasnia"
- University: "Manarat International University"

**About Me Section:**
- Edit the paragraph text with your personal story
- Update skills and interests as needed

**Education Section:**
- Update degree information, institutions, and dates
- Replace institution names with your actual education history

**Research Interests:**
- Edit the tag pills to match your research areas
- Add/remove research interest tags

**Leadership and Experience:**
- Update role titles, institutions, and dates
- Replace descriptions with your actual experience

**Skills:**
- Update skill names and proficiency levels
- The skill bars show percentage fill (0-100%)

### 5. Add/Remove Certificates
The Certificates section includes 3 certificate slots. To add/remove:
- Edit the HTML in the Certificates section
- Update the links to point to your actual PDF files in `assets/pdfs/`
- Each certificate has: badge icon, title, institution, and year

### 6. GitHub Pages Publishing

#### Option A: User/Organization Pages
1. Create a repository named `yourusername.github.io`
2. Push all files to the `main` branch
3. The site will be available at `https://yourusername.github.io`

#### Option: Project Pages
1. Create any repository name
2. Go to Settings > Pages
2. Select branch: `main` / `root` / `/ (root)`
3. The site will be available at `https://yourusername.github.io/repository-name`

#### Custom Domain:
1. In GitHub Pages settings, set a custom domain
2. Create a `CNAME` file in the root with your domain name
3. Configure DNS settings with your domain provider

## File Details

### index.html
- Semantic HTML5 structure with accessible elements
- Full responsive design with mobile-first approach
- 11 sections as specified
- Mobile navigation menu (hamburger → close ×)
- Anchor links with smooth scrolling
- Focus-visible states for keyboard navigation
- All paths are relative for GitHub Pages compatibility

### style.css
- Minimalist academic aesthetic
- Mobile-responsive with max-width constraints
- Focus-visible states and skip links
- Subtle animations on hover and scroll
- CSS variables for easy color customization
- Print-friendly styles for CV PDF

### script.js
- Mobile navigation toggle (hamburger menu)
- Smooth scroll for anchor links
- Reveal-on-scroll animations with IntersectionObserver
- Active navigation link highlighting on scroll
- Skill bar animation on view

## Customization Tips

### Adding More Certificates
```html
<!-- Add inside the certificates grid -->
<div class="certificate-card">
    <div class="certificate-badge">
        <svg>...</svg>
    </div>
    <div class="certificate-details">
        <h4>Certificate Title</h4>
        <p>Issuing Institution</p>
        <p>2024</p>
        <a href="assets/pdfs/my-certificate.pdf" class="btn btn--secondary">View Certificate</a>
    </div>
</div>
```

### Changing Colors
Update CSS variables in `:root`:
```css
:root {
    --teal-dark: #142D2B;
    --ivory: #F5F3EE;
    --gold-muted: #B49A78;
    --charcoal: #30343B;
    --white: #FFFFFF;
}
```

### Adding More Skills
```html
<div class="skill-bar">
    <span class="skill-name">Your Skill</span>
    <div class="skill-fill" style="width: 80%;"></div>
</div>
```

## License
Free to use and modify for personal academic purposes.