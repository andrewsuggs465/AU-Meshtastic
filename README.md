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

#### Deploy to GitHub Pages

1. Build the static site:

   ```bash
   zensical build
   ```

2. Push the generated `site/` directory to your GitHub repository:

   ```bash
   git add site/
   git commit -m "Build site"
   git push origin main
   ```

3. Configure GitHub Pages:
   - Go to your repository **Settings** → **Pages**
   - Set **Source** to "Deploy from a branch"
   - Select **main** branch and **/root** folder (or the folder containing your built site)
   - Click **Save**

The site will be deployed to `https://<username>.github.io/<repo-name>`
