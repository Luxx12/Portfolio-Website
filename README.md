# Gabriel Barreto Otero - Portfolio Website

A minimalist portfolio website with a bright, desert-inspired aesthetic featuring an abstract dune landscape and right-side navigation. Built with React and Tailwind CSS.

## 🏜️ Design Philosophy

**Bright Desert Minimalism:**
- **Light Color Palette**: Warm ambers, soft oranges, and stone tones on bright backgrounds
- **Abstract Desert Landscape**: SVG-based dune shapes on the home page create an artistic, flowing atmosphere
- **Right-Side Navigation**: Vertical navigation bar fixed to the right with minimalist styling
- **Generous Spacing**: Clean, airy layouts with plenty of breathing room
- **Light Typography**: Extralight and light font weights with wide letter spacing

**Key Features:**
- **Three Main Sections**:
  - **Home**: Abstract desert dune landscape background with profile and skills
  - **Journey**: Clean timeline with colored dot markers
  - **Projects**: Bordered cards with semi-transparent backgrounds

## 🎨 Color Palette

**Bright Theme:**
- **Backgrounds**: Amber-50, Orange-50, Stone-50/100 - Warm, light backgrounds
- **Cards**: White/40 with backdrop blur - Semi-transparent glassmorphism
- **Primary Text**: Stone-800 (#1c1917) - Deep warm brown
- **Secondary Text**: Stone-600/700 - Medium warm grays
- **Accents**: Amber-600/700/800 (#d97706, #b45309) - Warm desert orange
- **Borders**: Amber-300/400 with low opacity - Soft, warm borders

**Navigation:**
- **Position**: Fixed right side, vertical layout
- **Background**: Amber-50 with backdrop blur
- **Active State**: Border-left indicator with amber-600

## 🚀 Quick Start

### Option 1: View Locally (Easiest)
1. Open `index.html` in your web browser
2. That's it! The site works without any installation

### Option 2: Deploy to GitHub Pages (Free Hosting)
1. Create a GitHub account (if you don't have one)
2. Create a new repository named `your-username.github.io`
3. Upload `index.html` to the repository
4. Your site will be live at `https://your-username.github.io`

### Option 3: Deploy to Netlify/Vercel (Also Free)
1. Sign up for Netlify (netlify.com) or Vercel (vercel.com)
2. Drag and drop the `index.html` file
3. Get a custom URL instantly!

## ✏️ How to Customize

All your personal information is at the **top of the file** in clearly marked sections. Here's what you can edit:

### 1. Profile Information (Lines 40-50 in index.html)
```javascript
const PROFILE = {
  name: "Gabriel Barreto Otero",  // Change your name
  title: "Computer Science Student @ UCF",  // Change your title
  image: "URL_TO_YOUR_PHOTO",  // Replace with your photo URL
  email: "barretgaby12@gmail.com",  // Your email
  github: "https://github.com/luxx12",  // Your GitHub
  linkedin: "https://linkedin.com/in/Gabriel-B-Otero",  // Your LinkedIn
  about: [
    "First paragraph about yourself",
    "Second paragraph",
    "Third paragraph"
  ]
};
```

### 2. Adding New Experiences to Journey (Lines 52-140 in index.html)

**To add a new experience:**
1. Find the `JOURNEY` array
2. Copy any existing item (like the education or work example)
3. Paste it at the end of the array
4. Update the details:

```javascript
{
  id: 7,  // Increment the ID number
  type: "work",  // Types: "education", "work", "leadership", "event", "project"
  title: "Your New Job Title",
  organization: "Company Name",
  location: "City, State",
  date: "Month Year - Month Year",
  description: "Brief description of what you did",
  highlights: [
    "Key achievement 1",
    "Key achievement 2",
    "Key achievement 3"
  ]
}
```

**Important:** Don't forget the comma before your new entry!

### 3. Adding New Projects (Lines 142-170 in index.html)

**To add a new project:**
1. Find the `PROJECTS` array
2. Copy an existing project
3. Paste it at the end
4. Update with your project details:

```javascript
{
  id: 3,  // Increment the ID
  title: "Your Project Name",
  description: "Detailed description of what your project does and the technologies used.",
  gif: "URL_TO_YOUR_GIF",  // URL to your project demo GIF
  tags: ["Tech1", "Tech2", "Tech3"],  // Technologies used
  github: "https://github.com/your-username/your-repo",  // GitHub repo link
  demo: "https://your-demo-link.com",  // Live demo link (or null if none)
  award: "Award Name"  // Optional: null if no award
}
```

### 4. Updating Skills (Lines 172-177 in index.html)

```javascript
const SKILLS = {
  languages: ["Java", "Python", "JavaScript"],  // Add/remove languages
  frameworks: ["React", "Node.js", "Flask"],  // Add/remove frameworks
  tools: ["Git", "VS Code", "Docker"],  // Add/remove tools
  apis: ["Google API", "OpenCV"]  // Add/remove APIs/libraries
};
```

## 📸 How to Get Your Photo URL

### Method 1: GitHub (Free & Easy)
1. Create a GitHub repository (can be private)
2. Upload your photo to the repository
3. Right-click the image and select "Copy image address"
4. Use that URL in the `image` field

### Method 2: Imgur (Free Image Hosting)
1. Go to imgur.com
2. Upload your image
3. Right-click the image and select "Copy image address"
4. Use that URL

### Method 3: Google Drive (If you have Google Drive)
1. Upload your photo to Google Drive
2. Right-click → Get link → Change to "Anyone with the link"
3. Use this format: `https://drive.google.com/uc?id=FILE_ID`
   (Replace FILE_ID with the ID from your share link)

## 🎬 How to Add Project GIFs

### Creating GIFs of Your Projects:
1. **For Web Apps:**
   - Use [ScreenToGif](https://www.screentogif.com/) (Windows)
   - Use [Kap](https://getkap.co/) (Mac)
   - Use [Peek](https://github.com/phw/peek) (Linux)

2. **For Mobile Apps:**
   - Record screen on your phone
   - Convert to GIF using [ezgif.com](https://ezgif.com/)

3. **Hosting Your GIFs:**
   - Upload to GitHub (same as photos)
   - Upload to Imgur
   - Upload to Giphy

**Pro Tip:** Keep GIFs under 5MB for faster loading. Use ezgif.com to optimize if needed.

## 🎨 Changing Colors

The site uses a Dune-inspired desert color palette. To customize the accent colors:

**Main Accent Color (currently amber/orange):**
- Find `amber-` throughout the code (e.g., `text-amber-600`, `border-amber-800`)
- Replace `amber` with other warm Tailwind colors:
  - `orange` (Warmer desert tones)
  - `yellow` (Lighter sand tones)
  - `stone` (More neutral, cooler)
  - `neutral` (Even more neutral)
  - `slate` (Cooler, bluish grays)

**Example Changes:**
- Navigation underline: `border-amber-500` → `border-orange-500`
- Section headers: `text-amber-600` → `text-yellow-600`

**Background Adjustment:**
- Current: `bg-stone-950` (warm black)
- Alternatives: `bg-neutral-950` (neutral black), `bg-slate-950` (cool black)

**Typography:**
- Font weight is intentionally light (`font-light`, `font-extralight`)
- Letter spacing is wide (`tracking-wide`, `tracking-widest`)
- Keep these for the minimalist aesthetic

**Pro Tip:** The Dune aesthetic relies on subtlety - keep opacity low (e.g., `/30`, `/40`, `/60`) for borders and accents to maintain the refined, minimalist look.

## 📱 Features

- ✅ Bright, desert-inspired minimalist aesthetic
- ✅ Abstract desert dune landscape on home page (SVG-based)
- ✅ Right-side vertical navigation bar
- ✅ Warm amber and stone color palette
- ✅ Generous white space and breathing room
- ✅ Light typography with wide letter spacing
- ✅ Fully responsive (works on phones, tablets, and desktops)
- ✅ Glassmorphism effects (semi-transparent cards with backdrop blur)
- ✅ Subtle borders and refined hover effects
- ✅ Minimal timeline with colored dot markers
- ✅ Clean project showcase with bordered cards
- ✅ Skills displayed with bullet separators (·)
- ✅ Vertical name display in navigation
- ✅ No installation required - just open in browser
- ✅ Easy to customize colors and content

## 🔧 Advanced: Using the React Component

If you want to use this in a React project:

1. Install dependencies:
```bash
npm install react react-dom lucide-react
npm install -D tailwindcss
```

2. Use the `portfolio.jsx` file in your React app

3. Import in your main app:
```javascript
import Portfolio from './portfolio';

function App() {
  return <Portfolio />;
}
```

## 📝 Maintenance Tips

### Regularly Update:
- ✅ Add new projects as you build them
- ✅ Update your journey with new experiences
- ✅ Keep your skills list current
- ✅ Update your profile photo annually

### Before Interviews:
- ✅ Review all content for typos
- ✅ Ensure all links work
- ✅ Test on mobile devices
- ✅ Update GPA if it changes

## 🐛 Troubleshooting

**Problem: Page is blank**
- Check browser console for errors (F12 → Console tab)
- Verify all quotes and commas in your arrays

**Problem: Layout looks broken**
- Clear your browser cache (Ctrl+F5)
- Try a different browser

**Problem: GIFs not loading**
- Verify the URL is accessible
- Try opening the GIF URL directly in your browser
- Use a different image host

**Problem: Want to add more than 3 skills sections**
- Copy the entire `<div>` block for a skill section
- Paste it in the grid
- Update the heading and skills array

## 📧 Need Help?

If you get stuck:
1. Double-check the comma placement in arrays
2. Make sure all quotes match (opening and closing)
3. Look for the error message in browser console (F12)
4. Ask ChatGPT or Claude for help with specific issues

## 🎓 What You've Built

This is a professional portfolio that:
- Shows your education and perfect 4.0 GPA
- Highlights your $20,000+ in hackathon winnings
- Displays your teaching experience with 280+ students
- Showcases your award-winning projects
- Demonstrates your technical skills across multiple languages
- Presents you as a well-rounded CS student

## 🚀 Next Steps

1. **Customize** with your photo and any additional information
2. **Test** on different devices and browsers
3. **Deploy** to GitHub Pages or Netlify
4. **Share** the link on your resume and LinkedIn
5. **Update** regularly as you gain more experience

Good luck, Gabriel! Your portfolio looks great! 🎉