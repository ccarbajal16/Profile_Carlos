# Carlos Carbajal Professional Profile

This is a personal professional profile website built with [Hugo](https://gohugo.io/) and deployed using GitHub Actions. This site showcases my professional experience and projects.

## Overview

This website serves as a professional portfolio showcasing skills, experience, and projects. It is built as a static site using Hugo and is automatically deployed to GitHub Pages whenever changes are pushed to the main branch.

## Local Development

### Prerequisites

- [Hugo Extended](https://gohugo.io/getting-started/installing/) (v0.91.2 or later)
- Git

### Running Locally

1. Clone this repository:
   ```
   git clone https://github.com/your-username/Profile_Carlos.git
   cd Profile_Carlos
   ```

2. Start the Hugo development server:
   ```
   hugo server -D
   ```

3. Open your browser and navigate to http://localhost:1313/

## Making Changes

### Content Structure

- **Content**: All content is in the `content/` directory
  - `content/home/`: Widgets that appear on the homepage
  - `content/project/`: Project details
  - Other sections like posts, publications, etc.

- **Static Assets**: Images and other static files are in the `static/` directory

### Adding a New Project

1. Create a new markdown file in `content/project/` directory:
   ```
   hugo new project/my-new-project.md
   ```

2. Edit the front matter and content of the file

3. Add any project images to `static/img/projects/`

### Customizing the Theme

- CSS customizations can be added to `static/css/custom.css`
- Configuration settings are in `config.toml`

## Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions. The workflow is defined in `.github/workflows/hugo-deploy.yml`.

### How it works

1. When you push changes to the `main` branch, GitHub Actions will:
   - Build the Hugo site
   - Deploy the generated files to GitHub Pages

2. The site will be available at: https://your-username.github.io/Profile_Carlos/

### Manual Deployment

If you need to trigger a deployment manually:

1. Go to the "Actions" tab in your GitHub repository
2. Select the "Deploy Hugo site to GitHub Pages" workflow
3. Click "Run workflow"

## Customization

### Changing Personal Information

1. Edit your personal details in `config.toml`
2. Update your biography in `content/home/about.md`
3. Update your skills in `content/home/skills.md`
4. Update your experience in `content/home/experience.md`

### Adding Social Media Links

Add or modify social media links in the `[[params.social]]` section of `config.toml`.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
