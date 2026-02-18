# SignalStack Documentation Platform

![Status](https://img.shields.io/badge/status-active-success.svg)
![Jekyll](https://img.shields.io/badge/jekyll-v4.3-red.svg)
![Ruby](https://img.shields.io/badge/ruby-3.4%2B-red.svg)

The official documentation hub for **SignalStack**, a real-time event and notification infrastructure platform. This repository hosts the static website source code, built with **Jekyll** and the **Just the Docs** theme.

---

## 🚀 Features

- **Versioned Documentation**: Separate content streams for `v1.0` (Legacy) and `v2.0` (Latest).
- **Dark Mode**: Custom "SignalStack Dark" theme (Deep Navy / Electric Blue) for a developer-centric aesthetic.
- **Search**: Built-in client-side search indexing.
- **Responsive Design**: Optimized for mobile, tablet, and desktop.
- **SEO Optimized**: Fully configured metadata and social sharing tags.

## 🛠 Tech Stack

- **Static Site Generator**: [Jekyll](https://jekyllrb.com/)
- **Theme**: [Just the Docs](https://just-the-docs.com/) (Remote Theme)
- **Language**: Ruby 3.4+ / Sass
- **Deployment**: GitHub Actions (GitHub Pages)

## 🏁 Quick Start

### Prerequisites

- **Ruby**: Version 3.2 or higher (3.4 recommended).
- **Bundler**: `gem install bundler`

### Local Development

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-org/signalstack-docs.git
    cd signalstack-docs
    ```

2.  **Install dependencies:**
    ```bash
    bundle install
    ```

3.  **Run the local server:**
    ```bash
    bundle exec jekyll serve
    ```

4.  **View the site:**
    Open `http://127.0.0.1:4000` in your browser.

> **Note:** If you modify `_config.yml`, you must restart the server for changes to take effect.

## 📂 Project Structure

```mermaid
graph TD;
    root[SignalStack Docs]
    root --> docs[docs/]
    docs --> v1[v1/ (Legacy Content)]
    docs --> v2[v2/ (Latest Content)]
    root --> sass[_sass/]
    sass --> custom[custom/ (Theme Overrides)]
    root --> assets[assets/]
    assets --> images[images/ (Favicons, Logos)]
    root --> config[_config.yml (Site Configuration)]
    root --> gemfile[Gemfile (Dependencies)]
```

- **`docs/`**: Contains the core documentation markdown files, organized by version.
- **`_sass/custom/`**:
    - `setup.scss`: Overrides theme variables (Colors, Typography).
    - `custom.scss`: Additional CSS adjustments.
- **`_config.yml`**: Main configuration for the Jekyll site (Title, Plugins, Navigation).

## 🚀 Deployment

This project is configured for **Continuous Deployment** to GitHub Pages via GitHub Actions.

1.  **Push changes** to the `main` branch.
2.  The workflow defined in `.github/workflows/jekyll.yml` will automatically:
    - Build the Jekyll site.
    - Upload the artifact.
    - Deploy to the `gh-pages` environment.

**Configuration:**
Ensure your GitHub repository settings have **Pages** source set to **GitHub Actions**.

## 🤝 Contributing

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/amazing-feature`).
3.  Commit your changes (`git commit -m 'Add amazing feature'`).
4.  Push to the branch (`git push origin feature/amazing-feature`).
5.  Open a Pull Request.

---

© 2024 SignalStack. All rights reserved.
