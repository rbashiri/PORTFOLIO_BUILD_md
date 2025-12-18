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

- Option A (fast + modern): Next.js + Tailwind (recommended)
1) Create the project
npx create-next-app@latest my-portfolio
cd my-portfolio
npm install
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

2) Configure Tailwind

tailwind.config.js

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./app/**/*.{js,ts,jsx,tsx}", "./components/**/*.{js,ts,jsx,tsx}"],
  theme: { extend: {} },
  plugins: [],
};


app/globals.css

@tailwind base;
@tailwind components;
@tailwind utilities;

html, body { height: 100%; }

3) Paste this page (matches your screenshot layout)

app/page.jsx

export default function Home() {
  return (
    <main className="min-h-screen bg-[#070a12] text-white">
      {/* Top Nav */}
      <header className="sticky top-0 z-50 border-b border-white/10 bg-[#070a12]/70 backdrop-blur">
        <div className="mx-auto flex max-w-5xl items-center justify-between px-5 py-4">
          <div className="flex items-center gap-3">
            <div className="grid h-9 w-9 place-items-center rounded-lg bg-violet-500/90 font-semibold">
              GT
            </div>
          </div>

          <nav className="hidden gap-6 text-sm text-white/80 md:flex">
            <a className="hover:text-white" href="#home">Home</a>
            <a className="hover:text-white" href="#about">About</a>
            <a className="hover:text-white" href="#skills">Skills</a>
            <a className="hover:text-white" href="#projects">Projects</a>
            <a className="hover:text-white" href="#contact">Contact</a>
            <a className="hover:text-white underline underline-offset-4" href="#resume">Resume</a>
            <button
              className="ml-2 rounded-full border border-white/15 px-2 py-1 text-xs hover:bg-white/5"
              title="Theme toggle (optional)"
            >
              🌙
            </button>
          </nav>
        </div>
      </header>

      {/* Content */}
      <section id="home" className="mx-auto max-w-5xl px-5 pb-24 pt-16">
        <h1 className="text-center text-3xl font-semibold tracking-tight md:text-5xl">
          Volunteer Experience
        </h1>

        <div className="mx-auto mt-10 max-w-3xl rounded-2xl border border-white/10 bg-white/5 p-7 shadow-[0_20px_80px_rgba(0,0,0,0.45)]">
          <h2 className="text-xl font-semibold md:text-2xl">
            Full-Stack Engineer — Murphy Foundation (Uganda)
          </h2>
          <p className="mt-2 text-sm text-white/60">
            2024 – Present • Remote Volunteer Role
          </p>

          <ul className="mt-5 list-disc space-y-3 pl-5 text-white/80">
            <li>Supported the development of digital tools used in educational programs.</li>
            <li>Improved UI flows for non-technical users in underserved communities.</li>
            <li>Collaborated with international teams on backend and frontend tasks.</li>
            <li>Contributed to scalable system improvements and documentation.</li>
          </ul>
        </div>
      </section>
    </main>
  );
}

4) Run it
npm run dev

5) Deploy (free)

Push to GitHub

Deploy on Vercel (1-click import from GitHub)
