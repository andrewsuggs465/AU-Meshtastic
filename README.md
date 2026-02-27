# Auburn University Meshtastic

A student-led community exploring Meshtastic, LoRa, and mesh networking at Auburn University.

## Quick Start

### Setup

1. Clone the repository and open in VS Code.
2. Create and activate a Python virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install Zensical (static site generator):

   ```bash
   pip install zensical
   ```

4. Serve the docs locally:

   ```bash
   zensical serve
   ```

   Then open <http://127.0.0.1:8000>

### Deployment

#### Automatic Deployment with GitHub Actions (Recommended)

The repository includes a GitHub Actions workflow that automatically deploys the `site/` folder to GitHub Pages when you push changes.

1. Build the site locally:

   ```bash
   zensical build
   ```

2. Commit and push your changes (including the updated `site/` folder):

   ```bash
   git add .
   git commit -m "Update content"
   git push origin main
   ```

3. GitHub Actions will automatically deploy the `site/` folder to GitHub Pages.

4. Your site will be available at `https://<username>.github.io/<repo-name>`
