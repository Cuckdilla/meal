# Weekly Meal Plan - Retype Site

A beautiful, responsive website for your personalized weekly meal plan, built with Retype and deployed on GitHub Pages.

## 🚀 Quick Start

### Prerequisites
- GitHub account
- Node.js (for local development)

### Local Development

1. **Install Retype**
   ```bash
   npm install -g retypeapp
   ```

2. **Clone the repository**
   ```bash
   git clone <your-github-repo-url>
   cd diet
   ```

3. **Build the site locally**
   ```bash
   retype build
   ```

4. **Preview the site**
   ```bash
   retype serve
   ```
   Then open http://localhost:3000 in your browser.

## 📁 Project Structure

```
diet/
├── retype.yml              # Retype configuration
├── index.md                # Home page
├── about.md                # About page
├── cutting/                # Cutting phase section
│   ├── index.md           # Cutting overview
│   ├── monday.md          # Monday meal plan
│   ├── tuesday.md         # Tuesday meal plan
│   ├── wednesday.md       # Wednesday meal plan
│   ├── thursday.md        # Thursday meal plan
│   ├── friday.md          # Friday meal plan
│   ├── saturday.md        # Saturday meal plan
│   └── sunday.md          # Sunday meal plan
├── .github/workflows/      # GitHub Actions
│   └── deploy.yml         # Deployment workflow
└── README.md              # This file
```

## 🌐 Deployment

The site is automatically deployed to GitHub Pages when you push to the `main` or `master` branch.

### Manual Deployment

1. **Push your changes**
   ```bash
   git add .
   git commit -m "Update meal plan"
   git push origin main
   ```

2. **Check the workflow**
   - Go to your GitHub repository
   - Navigate to Actions tab
   - Monitor the build and deploy workflow

3. **Access your site**
   - Your site will be available at: `https://<username>.github.io/<repository-name>`
   - Enable GitHub Pages in repository settings if needed

## 🎨 Customization

### Theme Colors
Edit `retype.yml` to change the primary color:
```yaml
theme:
  primary: "#3b82f6"  # Change this to your preferred color
```

### Navigation
Modify the navigation in `retype.yml`:
```yaml
nav:
  - title: Home
    url: /
  - title: Cutting
    url: /cutting
    children:
      - title: Overview
        url: /cutting
      - title: Monday
        url: /cutting/monday
      # ... other days
```

### Adding New Phases
To add bulking or maintenance plans:

1. Create a new folder (e.g., `bulking/`)
2. Add individual day files
3. Update `retype.yml` with new navigation
4. Add the new section to the pages list

## 📱 Features

- **Responsive design** - works on all devices
- **Search functionality** - find meals quickly
- **Dark/light mode** - toggle theme
- **Fast loading** - optimized static site
- **SEO friendly** - proper meta tags and structure
- **Organized sections** - easy to add bulking/maintenance plans

## 🔧 Troubleshooting

### Build Issues
- Ensure all `.md` files referenced in `retype.yml` exist
- Check that the YAML syntax is correct
- Verify Node.js version (18+ recommended)

### Deployment Issues
- Check GitHub Actions workflow logs
- Ensure GitHub Pages is enabled in repository settings
- Verify the workflow is running on the correct branch

## 📝 Updating the Meal Plan

1. Edit the specific day files in the `cutting/` folder
2. Update the summary table in `cutting/index.md` if needed
3. Commit and push your changes
4. The site will automatically rebuild and deploy

## 🎯 Future Plans

- [ ] Add bulking phase meal plans
- [ ] Add maintenance phase meal plans
- [ ] Include meal prep instructions
- [ ] Add shopping list generation
- [ ] Create printable PDF versions
- [ ] Add meal photos

## 📊 Current Structure

### Cutting Phase
- **Daily targets:** 1,900 kcal, 182g protein, 84g fat, 104g carbs
- **Weekly average:** 2,029 kcal, 175.8g protein, 83.7g fat, 158.1g carbs
- **Features:** Overnight oats, Greek yogurt, meal prep lunches

---

**Happy meal planning! 🥗** 