# PORTFOLIO_BUILD_md
Option 2: Save as a simple checklist (very low effort)

Copy this into Notes / Google Docs / Notion:

Portfolio – Build Later

 Use Next.js + Tailwind

 Dark theme + top navbar

 Volunteer Experience card

 Sections: About, Skills, Projects

 Resume PDF link

 Deploy on Vercel
 # Portfolio – Build Later Notes

## Goal
Recreate a dark-themed portfolio website with:
- Top navigation bar
- Sections: Home, About, Skills, Projects, Contact, Resume
- Card-style “Volunteer Experience” section
- Clean, modern UI (similar to Gisell Tavarez portfolio)

## Tech Stack (chosen)
- Next.js
- Tailwind CSS
- Deployed on Vercel

## Steps to Build (When Ready)

### 1. Create project
npx create-next-app@latest my-portfolio  
cd my-portfolio

### 2. Install Tailwind
npm install -D tailwindcss postcss autoprefixer  
npx tailwindcss init -p

### 3. Configure Tailwind
- Edit `tailwind.config.js`
- Add Tailwind to `globals.css`

### 4. Build main layout
- Dark background
- Sticky top navbar
- Initials logo (top-left)
- Section anchors (Home, About, Skills, Projects, Contact, Resume)

### 5. Volunteer Experience card
- Rounded card
- Role title
- Dates + remote note
- Bullet points describing impact

### 6. Deploy
- Push to GitHub
- Deploy with Vercel (free)

## Customization TODO
- Replace initials with my own
- Add my real experience
- Upload resume PDF
- Add Projects section
