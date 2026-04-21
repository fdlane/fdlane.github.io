# fdlane.github.io

Personal site for [fdlane.com](https://www.fdlane.com/), hosted on GitHub Pages.

## Tech Stack

- Static HTML
- [Tailwind CSS v4](https://tailwindcss.com/) (compiled via standalone CLI)
- GitHub Pages (deployment)

## Local Development

### 1. Download the Tailwind standalone CLI (one-time setup)

```bash
curl -sLO https://github.com/tailwindlabs/tailwindcss/releases/latest/download/tailwindcss-linux-x64
chmod +x tailwindcss-linux-x64
```

### 2. Build CSS

```bash
./tailwindcss-linux-x64 -i src/input.css -o assets/css/styles.css --minify
```

Or watch for changes during development:

```bash
./tailwindcss-linux-x64 -i src/input.css -o assets/css/styles.css --watch
```

### 3. Serve locally

```bash
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080/). Refresh after file changes.

## Deployment

Push to the `main` branch. GitHub Pages will serve the site automatically (Jekyll is disabled via `.nojekyll`).

Remember to rebuild CSS before committing if you changed any Tailwind classes or the input CSS.

## Project Structure

```
index.html              Main site — hero, services, SevereClear
about.html              About page
404.html                Custom 404 page
CNAME                   Custom domain config
.nojekyll               Disables Jekyll processing
src/
  input.css             Tailwind input (theme config)
assets/
  css/styles.css        Compiled Tailwind output
  images/               Profile photo, logos
```

# fdlane.github.io

Personal site built with Jekyll and Tailwind CSS, hosted on GitHub Pages.

## Prerequisites

- [Git](https://git-scm.com/)
- [Docker](https://docker.com/)

## Running Locally

```bash
docker compose up
```

Visit [http://localhost:4000](http://localhost:4000).

Jekyll watches for file changes and rebuilds automatically. Refresh the browser to see updates.

## Deploying

Push to the `main` branch. GitHub Pages builds and deploys automatically.
