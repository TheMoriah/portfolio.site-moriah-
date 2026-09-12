# Moriah Chiang — Portfolio

Personal portfolio site for Moriah Chiang, Freelance Digital Product Designer.

## Tech Stack

- **React 19** + **Vite**
- **React Router v7** — client-side routing
- **CSS** (custom properties, no Tailwind utilities)
- **Montserrat** font via Google Fonts

## Running This Locally (No Coding Experience Needed)

These steps let you view and test the site on your own computer, before anything goes live.

### 1. Install Node.js (one-time setup)

Node.js is the program that lets your computer run this website's code.

1. Go to [nodejs.org](https://nodejs.org)
2. Download the **LTS** version (the one recommended for most people)
3. Open the downloaded file and click through the installer (defaults are fine)

To check it worked, open your computer's terminal app:
- **Mac**: press `Cmd + Space`, type `Terminal`, hit Enter
- **Windows**: press the Start key, type `Command Prompt`, hit Enter

Type this and press Enter:
```bash
node -v
```
If you see a version number (like `v22.0.0`), you're good to go.

### 2. Get the project files

If you don't already have the project folder on your computer, download it from GitHub:
1. Go to the repository page on GitHub
2. Switch to the `moriah-portifolio-1` branch using the branch dropdown near the top-left of the file list (it defaults to `main`, so make sure to change it)
3. Click the green **Code** button → **Download ZIP**
4. Unzip it somewhere easy to find, like your Desktop

### 3. Open a terminal in the project folder

In the terminal, navigate into the `moriah-portfolio` folder. For example, if you unzipped it to your Desktop:
```bash
cd Desktop/portfolio.site-moriah-/moriah-portfolio
```

### 4. Install the project's dependencies (one-time per download)

```bash
npm install
```
This downloads everything the site needs to run. It's normal for this to take a minute or two, and to see some yellow warning text — that's fine, as long as it finishes without a red "error".

### 5. Start the site

```bash
npm run dev
```
After a few seconds you'll see something like:
```
Local:   http://localhost:5173/
```
Open that link in your browser (Cmd/Ctrl + click it, or copy-paste it) — the site is now running on your computer. Any changes made to the code will show up automatically while this is running.

To stop it, click back in the terminal and press `Ctrl + C`.

### Other commands

```bash
# Build a production-ready version (creates a "dist" folder)
npm run build

# Preview that production build locally
npm run preview
```

## Project Structure

```
src/
├── assets/          # SVGs, images, resume PDF
├── components/
│   ├── Header.jsx   # Top nav + work page hero section
│   ├── Footer.jsx   # Bottom nav + contact info + LinkedIn
│   └── ProjectCard.jsx
├── pages/
│   ├── WorkPage.jsx  # Project listing
│   └── AboutPage.jsx # Bio, photo, skills & tools
├── App.jsx
├── App.css          # All styles + responsive breakpoints
└── index.css        # Global reset + font import
```

## Pages

| Route | Description |
|-------|-------------|
| `/` or `/work` | Work page — lists all projects |
| `/about` | About page — bio, skills, tools, resume |

## Responsive Breakpoints

| Breakpoint | Layout |
|------------|--------|
| > 900px | Desktop — full side-by-side layouts |
| ≤ 900px | Tablet — condensed grid, single-column skills |
| ≤ 600px | Mobile — stacked cards, hamburger nav |

## Planned Next Steps

- Project detail pages (linked from "View Me" buttons)
- Services page
- Contact section / form
