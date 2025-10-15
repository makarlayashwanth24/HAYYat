<p align="center">
    <h1 align="center">HAYYat</h1>
</p>
<p align="center">
    <em>News sentiment analyzer with a simple static frontend</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/makarlayashwanth24/HAYYat?style=flat&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/makarlayashwanth24/HAYYat?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/makarlayashwanth24/HAYYat?style=flat&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/makarlayashwanth24/HAYYat?style=flat&color=0080ff" alt="repo-language-count">
</p>
<p align="center">
		<em>Built with the tools and technologies:</em>
</p>
<p align="center">
	<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat&logo=JavaScript&logoColor=black" alt="JavaScript">
	<img src="https://img.shields.io/badge/HTML5-E34F26.svg?style=flat&logo=HTML5&logoColor=white" alt="HTML5">
	<img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white" alt="Python">
	<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white" alt="GitHub%20Actions">
	<img src="https://img.shields.io/badge/pandas-150458.svg?style=flat&logo=pandas&logoColor=white" alt="pandas">
	<img src="https://img.shields.io/badge/JSON-000000.svg?style=flat&logo=JSON&logoColor=white" alt="JSON">
</p>

<br>

##### 🔗 Table of Contents

- [📍 Overview](#-overview)
- [👾 Features](#-features)
- [📂 Repository Structure](#-repository-structure)
- [🧩 Modules](#-modules)
- [🚀 Getting Started](#-getting-started)
    - [🔖 Prerequisites](#-prerequisites)
    - [📦 Installation](#-installation)
    - [🤖 Usage](#-usage)
    - [🧪 Tests](#-tests)
- [📌 Project Roadmap](#-project-roadmap)
- [🤝 Contributing](#-contributing)
- [🎗 License](#-license)
- [🙌 Acknowledgments](#-acknowledgments)

---

## 📍 Overview

HAYYat collects the latest news, analyzes sentiment, and exposes the results to a lightweight static UI.

- Python script (`app.py`) scrapes category pages (e.g., India Today for Business, Entertainment, Sports, Education) and can be extended to Google News RSS.
- Sentiment is computed with TextBlob's PatternAnalyzer and stored as Positive/Negative.
- Output is written into a compact JSON file (`news_data.json`) grouped by category for easy consumption by the frontend.
- The frontend is a static landing page (`index.html`) with category pages and smooth-scrolling UX.

---

## 👾 Features

- Scrape news from multiple categories
- Optional Google News RSS parsing (helper included, currently commented in `app.py`)
- Sentiment analysis via TextBlob PatternAnalyzer
- Aggregated output JSON per category with sentiment, URL, and headline
- Static UI with fullscreen video hero and category tiles
- No server required to view the UI; generate data once, then open `index.html`

---

## 📂 Repository Structure

```sh
└── HAYYat/
    ├── .github
    │   └── workflows
    │       └── main.yml
    ├── 1793334-hd_1920_1080_30fps.mp4
    ├── 2022396-hd_1920_1080_30fps.mp4
    ├── 3192198-uhd_3840_2160_25fps.mp4
    ├── 5905282-hd_1920_1080_24fps.mp4
    ├── 5983185-uhd_3840_2160_30fps.mp4
    ├── app.py
    ├── business.css
    ├── business.html
    ├── business.js
    ├── education.css
    ├── education.html
    ├── education.js
    ├── entertainment.css
    ├── entertainment.html
    ├── entertainment.js
    ├── index.html
    ├── logo.jpg
    ├── news_data.json
    ├── news_data2.json
    ├── pexels-emily-ranquist-493228-1205651.jpg
    ├── pexels-sebastian-ervi-866902-1763075.jpg
    ├── pexels-tranmautritam-233129.jpg
    ├── politics.jpg
    ├── requirements.txt
    ├── script.js
    ├── sports.css
    ├── sports.html
    ├── sports.jpg
    ├── sports.js
    └── styles.css
```

---

## 🧩 Modules

<details closed><summary>.</summary>

| File | Summary |
| --- | --- |
| [news_data2.json](https://github.com/makarlayashwanth24/HAYYat/blob/main/news_data2.json) | Sample data variant (if present) |
| [news_data.json](https://github.com/makarlayashwanth24/HAYYat/blob/main/news_data.json) | Generated news with sentiment grouped by category |
| [styles.css](https://github.com/makarlayashwanth24/HAYYat/blob/main/styles.css) | Global styles for landing page and layout |
| [index.html](https://github.com/makarlayashwanth24/HAYYat/blob/main/index.html) | Landing page with video hero and category links |
| [business.css](https://github.com/makarlayashwanth24/HAYYat/blob/main/business.css) | Styles for Business page |
| [business.html](https://github.com/makarlayashwanth24/HAYYat/blob/main/business.html) | Business category UI |
| [business.js](https://github.com/makarlayashwanth24/HAYYat/blob/main/business.js) | Business page behavior (reads JSON, renders items) |
| [script.js](https://github.com/makarlayashwanth24/HAYYat/blob/main/script.js) | Landing page interactions (fade-in, smooth scroll) |
| [entertainment.js](https://github.com/makarlayashwanth24/HAYYat/blob/main/entertainment.js) | Entertainment page behavior |
| [sports.html](https://github.com/makarlayashwanth24/HAYYat/blob/main/sports.html) | Sports category UI |
| [sports.js](https://github.com/makarlayashwanth24/HAYYat/blob/main/sports.js) | Sports page behavior |
| [entertainment.css](https://github.com/makarlayashwanth24/HAYYat/blob/main/entertainment.css) | Styles for Entertainment page |
| [entertainment.html](https://github.com/makarlayashwanth24/HAYYat/blob/main/entertainment.html) | Entertainment category UI |
| [education.css](https://github.com/makarlayashwanth24/HAYYat/blob/main/education.css) | Styles for Education page |
| [sports.css](https://github.com/makarlayashwanth24/HAYYat/blob/main/sports.css) | Styles for Sports page |
| [education.html](https://github.com/makarlayashwanth24/HAYYat/blob/main/education.html) | Education category UI |
| [requirements.txt](https://github.com/makarlayashwanth24/HAYYat/blob/main/requirements.txt) | Python dependencies for scraping and sentiment |
| [app.py](https://github.com/makarlayashwanth24/HAYYat/blob/main/app.py) | Scraper + sentiment pipeline that outputs JSON |
| [education.js](https://github.com/makarlayashwanth24/HAYYat/blob/main/education.js) | Education page behavior |

</details>

<details closed><summary>.github.workflows</summary>

| File | Summary |
| --- | --- |
| [main.yml](https://github.com/makarlayashwanth24/HAYYat/blob/main/.github/workflows/main.yml) | CI configuration (if present) |

</details>

---

## 🚀 Getting Started

### 🔖 Prerequisites

• Python 3.9+
• pip
• Optional: VS Code Live Server or any static file server

### 📦 Installation

Build the project from source:

1. Clone the HAYYat repository:
```sh
❯ git clone https://github.com/makarlayashwanth24/HAYYat
```

2. Navigate to the project directory:
```sh
❯ cd HAYYat
```

3. Install the required dependencies:
```sh
❯ pip install -r requirements.txt
```

### 🤖 Usage

There are two parts: generate the data, then view the UI.

1) Generate or refresh news data (writes `news_data.json`):
```sh
❯ python app.py
```

2) Open the static site:
- Easiest: open `index.html` directly (double-click or from VS Code “Open with Live Server”).
- Or serve locally (from repo root):
```sh
❯ python -m http.server 8000
```
Then browse to `http://localhost:8000/`.

### 🧪 Tests

Execute the test suite using the following command:

```sh
❯ # No automated tests yet
```

---

## 📌 Project Roadmap

- [ ] Add live API endpoint to serve JSON dynamically
- [ ] Enrich scraping with more sources and pagination
- [ ] Improve sentiment labeling and add neutral class
- [ ] Add automated tests and CI

---

## 🤝 Contributing

Contributions are welcome! Here are several ways you can contribute:

- **[Report Issues](https://github.com/makarlayashwanth24/HAYYat/issues)**: Submit bugs or feature requests.
- **Submit Pull Requests**: Review open PRs, and submit your own PRs.
- **[Discussions](https://github.com/makarlayashwanth24/HAYYat/discussions)**: Share insights, feedback, or questions.

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/makarlayashwanth24/HAYYat
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to github**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!
</details>

<details closed>
<summary>Contributor Graph</summary>
<br>
<p align="left">
   <a href="https://github.com{/makarlayashwanth24/HAYYat/}graphs/contributors">
      <img src="https://contrib.rocks/image?repo=makarlayashwanth24/HAYYat">
   </a>
</p>
</details>

---

## 🎗 License

If a LICENSE file is not present, this project has no explicit license. Consider adding one from [Choose a License](https://choosealicense.com/licenses).

---

## 🙌 Acknowledgments

- List any resources, contributors, inspiration, etc. here.

---
