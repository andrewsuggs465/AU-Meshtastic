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

The repository includes a GitHub Actions workflow that automatically builds and deploys the site to GitHub Pages when you push to `main` or `master`.

1. Commit and push your changes:

   ```bash
   git add .
   git commit -m "Update content"
   git push origin main
   ```

2. GitHub Actions will automatically:
   - Build the site with Zensical
   - Deploy to GitHub Pages

3. Your site will be available at `https://<username>.github.io/<repo-name>`

#### Manual Deployment

If you prefer to deploy manually:

1. Build the static site:

   ```bash
   zensical build
   ```

2. Commit and push the `site/` directory:

   ```bash
   git add site/
   git commit -m "Build site"
   git push origin main
   ```

3. Configure GitHub Pages in repository **Settings** → **Pages**:
   - Set **Source** to "Deploy from a branch"
   - Select the branch and **`/site`** folder
   - Click **Save**
