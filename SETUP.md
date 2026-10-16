# 🚀 MrWhiiteHat Profile Deployment & Customization Guide

This guide provides complete instructions for configuring, deploying, and personalizing the next-generation cyber-themed GitHub Profile README for **`MrWhiiteHat`**.

---

## 📑 Table of Contents
1. [How GitHub Profile READMEs Work](#1-how-github-profile-readmes-work)
2. [Step-by-Step Deployment](#2-step-by-step-deployment)
3. [Repository File Structure](#3-repository-file-structure)
4. [Customization Guide](#4-customization-guide)
   - [Updating Project Repositories](#updating-project-repositories)
   - [Updating Contact & Social Links](#updating-contact--social-links)
   - [Modifying Cyber Theme Colors & SVGs](#modifying-cyber-theme-colors--svgs)
   - [Editing Terminal Bio & Personal Details](#editing-terminal-bio--personal-details)
5. [External Analytics & Telemetry Services](#5-external-analytics--telemetry-services)
6. [Automated Daily Cache-Busting Workflow](#6-automated-daily-cache-busting-workflow)
7. [Troubleshooting & FAQ](#7-troubleshooting--faq)

---

## 1. How GitHub Profile READMEs Work

GitHub provides a special feature: when you create a public repository with the exact same name as your GitHub username, the `README.md` in that repository's default branch (`main` or `master`) is automatically displayed at the top of your public GitHub user profile.

- **Account Username:** `MrWhiiteHat`
- **Target Repository Name:** `MrWhiiteHat` (Case-insensitive, but matches `https://github.com/MrWhiiteHat/MrWhiiteHat`)
- **Visibility:** Must be set to **Public**
- **Default Branch:** `main`

---

## 2. Step-by-Step Deployment

### Step 1: Create the Special Repository on GitHub
1. Log in to your GitHub account: [`https://github.com/MrWhiiteHat`](https://github.com/MrWhiiteHat).
2. Go to **Repositories** &rarr; **New** (or visit [`https://github.com/new`](https://github.com/new)).
3. In the **Repository name** field, enter:
   ```text
   MrWhiiteHat
   ```
   *(GitHub will display a banner: "You found a secret! MrWhiiteHat/MrWhiiteHat is a special repository that you can use to add a README.md to your GitHub profile.")*
4. Ensure **Public** is selected.
5. You can leave "Initialize this repository with a README" unchecked, since you will push this repository directly.
6. Click **Create repository**.

---

### Step 2: Initialize or Clone the Repository Locally

#### Option A: Pushing an Existing Local Directory
If you have these files locally in your workspace:
```bash
# Navigate to the workspace directory
cd "C:\Users\MrWhiteHat\Desktop\New folder"

# Initialize git if not already initialized
git init -b main

# Add the remote origin
git remote add origin https://github.com/MrWhiiteHat/MrWhiiteHat.git

# Stage all files (README.md, assets, .github, SETUP.md)
git add .

# Create initial commit
git commit -m "feat: initialize next-gen cyber profile"

# Push to GitHub
git push -u origin main
```

#### Option B: Cloning the Empty Repository First
```bash
git clone https://github.com/MrWhiiteHat/MrWhiiteHat.git
cd MrWhiiteHat

# Copy all profile files into this directory:
# - README.md
# - SETUP.md
# - assets/ (all 10 SVG files)
# - .github/workflows/stats-update.yml

git add .
git commit -m "feat: initialize next-gen cyber profile"
git push origin main
```

---

### Step 3: Enable GitHub Actions Workflow Permissions
To allow the automated cache-refresh workflow (`.github/workflows/stats-update.yml`) to commit and push timestamp updates:

1. In your `MrWhiiteHat/MrWhiiteHat` repository, navigate to **Settings**.
2. In the left sidebar, click **Actions** &rarr; **General**.
3. Scroll down to **Workflow permissions**.
4. Select **Read and write permissions**.
5. Check **Allow GitHub Actions to create and approve pull requests** (optional, recommended).
6. Click **Save**.

---

## 3. Repository File Structure

Ensure all assets and configuration files are located in the following relative directory structure:

```text
MrWhiiteHat/
├── .github/
│   └── workflows/
│       └── stats-update.yml      # GitHub Actions daily cache-busting runner
├── assets/
│   ├── about-terminal.svg        # Terminal window with identity details (850px)
│   ├── contact-panel.svg         # Holographic communications matrix (850px)
│   ├── divider-cyber.svg         # Animated glowing cyber divider line (900px)
│   ├── footer-terminal.svg       # Session termination terminal footer (850px)
│   ├── globe-hologram.svg        # Rotating wireframe globe hologram (400px)
│   ├── hero-banner.svg           # High-impact animated cyberpunk hero banner (900px)
│   ├── project-aegisai.svg       # Project card: AegisAI Cyber Defense (850px)
│   ├── project-msa.svg           # Project card: Mobile Security Agent (850px)
│   ├── project-realfake.svg      # Project card: RealFake Multimodal Detection (850px)
│   └── tech-grid.svg             # Categorized tech matrix grid (850px)
├── README.md                     # Assembled GitHub Profile page
└── SETUP.md                      # Deployment & maintenance guide
```

---

## 4. Customization Guide

### Updating Project Repositories
In `README.md`, find the `SECTION: MISSION CONTROL` block. Replace the placeholder links with your real repositories:

```html
<!-- UPDATE: Replace with actual repository URL -->
<a href="https://github.com/MrWhiiteHat/mobile-security-agent">
  <img src="assets/project-msa.svg" alt="Mobile Security Agent" width="850"/>
</a>

<!-- UPDATE: Replace with actual repository URL -->
<a href="https://github.com/MrWhiiteHat/aegisai">
  <img src="assets/project-aegisai.svg" alt="AegisAI Autonomous Cyber Defense" width="850"/>
</a>

<!-- UPDATE: Replace with actual repository URL -->
<a href="https://github.com/MrWhiiteHat/realfake-detection">
  <img src="assets/project-realfake.svg" alt="RealFake Multimodal Deepfake Detection" width="850"/>
</a>
```

### Updating Contact & Social Links
In `README.md`, find the `SECTION: ESTABLISH CONNECTION` block. Customize the shields badge URLs:

```markdown
<!-- UPDATE: Replace with actual LinkedIn profile -->
<a href="https://linkedin.com/in/YOUR_LINKEDIN_USERNAME" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn Profile"/>
</a>

<!-- UPDATE: Replace with actual contact email address -->
<a href="mailto:your_email@example.com">
  <img src="https://img.shields.io/badge/Encrypted_Mail-Secure_Channel-00ff88?style=flat-square&logo=minutemailer&logoColor=0d1117" alt="Direct Secure Email"/>
</a>
```

### Modifying Cyber Theme Colors & SVGs
All vector assets in `assets/*.svg` follow a unified cyberpunk color palette. To re-theme or tweak accents, search and replace hex codes within the SVG files:

| Element / Purpose | Color Name | Hex Code |
| :--- | :--- | :--- |
| **Primary Accent / Neon Green** | Cyber Green | `#00ff88` |
| **Secondary Accent / Cyan** | Electric Cyan | `#00e5ff` |
| **Tertiary Accent / Violet** | Neon Purple | `#7c4dff` |
| **Dark Base Background** | Void Canvas | `#0d1117` |
| **Card & Container Background** | Surface Slate | `#161b22` |
| **Borders & Grid Dividers** | Border Gray | `#30363d` |
| **Primary Terminal Text** | Pure White / Ice | `#e6edf3` |
| **Muted Telemetry / Labels** | Muted Silver | `#8b949e` |

### Editing Terminal Bio & Personal Details
- Open `assets/about-terminal.svg` in any code editor.
- Look for `<text>` tags containing terminal outputs:
  - System version, kernel parameters, current affiliations
  - Research focus, active defense initiatives, and mission briefing
- Modify the text directly inside `<tspan>` or `<text>` tags. Keep line lengths within 70 characters to avoid clipping.

---

## 5. External Analytics & Telemetry Services

The `README.md` leverages high-reputation, open-source dynamic analytics generators:

1. **GitHub Readme Stats** (by Anurag Hazra)
   - URL: `https://github-readme-stats.vercel.app`
   - Generates overall star count, commit count, PRs, issues, and contributed repositories.
   - Theme configured: `radical` with custom hex parameters `#0d1117`, `#00ff88`, `#00e5ff`.

2. **GitHub Readme Streak Stats** (by DenverCoder1)
   - URL: `https://github-readme-streak-stats.herokuapp.com`
   - Displays continuous contribution streaks, total contributions, and current streak records.

3. **Top Languages Card** (by Anurag Hazra)
   - URL: `https://github-readme-stats.vercel.app/api/top-langs/`
   - Automatically computes language usage ratios across your repositories.

4. **GitHub Activity Graph** (by Ashutosh00710)
   - URL: `https://github-readme-activity-graph.vercel.app`
   - Generates an SVG telemetry area chart of commit cadence throughout the year.

5. **Profile Views Counter** (by Anton Komarev)
   - URL: `https://komarev.com/ghpvc/`
   - Increments every time your profile is loaded.

> [!NOTE]
> All dynamic stats services are hosted on public infrastructure. If GitHub's image cache (`camo.githubusercontent.com`) or a third-party service experiences brief downtime, the alt text will be displayed cleanly until service resumes.

---

## 6. Automated Daily Cache-Busting Workflow

GitHub caches external images aggressively using a proxy service (`Camo`). To ensure that stats cards reflect updated numbers without remaining stale for days, the workflow at `.github/workflows/stats-update.yml` triggers once daily at `06:00 UTC`:

```yaml
name: Refresh Profile Stats Cache
on:
  schedule:
    - cron: '0 6 * * *'  # Daily at 6 AM UTC
  workflow_dispatch:     # Allows manual trigger via GitHub Actions tab

permissions:
  contents: write

jobs:
  refresh:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Update timestamp
        run: |
          echo "Last refreshed: $(date -u)" > .last-refresh
      - name: Commit changes
        run: |
          git config user.name 'github-actions[bot]'
          git config user.email 'github-actions[bot]@users.noreply.github.com'
          git add .last-refresh
          git diff --cached --quiet || git commit -m 'chore: refresh profile stats cache'
          git push
```

You can also trigger it manually at any time under the **Actions** tab on GitHub by clicking **Refresh Profile Stats Cache** &rarr; **Run workflow**.

---

## 7. Troubleshooting & FAQ

### Q: Why is my profile README not appearing on my profile page?
- Verify that your repository is named exactly `MrWhiiteHat` (case-insensitive, matching your GitHub username).
- Check that repository visibility is set to **Public** (Private profile repos are not rendered publicly).
- Ensure the file is named `README.md` (all capitals except `.md`) and is located in the root folder of branch `main`.

### Q: Why do some SVGs look static or fail to render animations?
- GitHub processes and sanitizes SVGs before serving them through its `camo` CDN proxy.
- GitHub sanitization strips all `<script>` tags, foreign objects, and external HTTP font declarations.
- All SVG assets provided in `assets/` use pure CSS keyframe animations (`@keyframes`) and system monospaced fonts (`ui-monospace`, `Courier New`, `monospace`), ensuring full compliance with GitHub's CSP (Content Security Policy).

### Q: Why did the GitHub Actions workflow fail with a permissions error?
- If the error reads: `remote: Permission to MrWhiiteHat/MrWhiiteHat.git denied to github-actions[bot]`, go to **Repository Settings** &rarr; **Actions** &rarr; **General** &rarr; **Workflow permissions**, and change it from *Read repository contents permission* to **Read and write permissions**.

### Q: How do the SVG cards render on mobile devices?
- Each image in `README.md` is bounded by HTML `width="..."` attributes and responsive SVG `viewBox` coordinate systems.
- GitHub's mobile app and responsive web views will automatically scale them down while maintaining full aspect ratios and crisp vector sharpness.

---

<p align="center">
  <sub><code>MrWhiiteHat &bull; Next-Gen Cyber Profile Architecture</code></sub>
</p>
