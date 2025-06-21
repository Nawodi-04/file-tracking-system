# Developer Guide – File Tracking System

This guide documents the internal structure, branches, roles, and contribution practices for the File Tracking System project.


## Project Overview

The **File Tracking System** is a frontend-only web application developed using HTML and CSS. It simulates a file management interface with forms, search features, and user navigation.


## Branch Strategy

Each feature or component was developed in a separate branch to ensure clean version control and easier collaboration.

| Branch Name        | Purpose                                 | File Created                         |
|--------------------|------------------------------------------|--------------------------------------|
| `login/register`   | Develop login and signup functionality   | `login.html`                         |
| `welcome`          | Create and style the welcome page        | `index.html`                       |
| `addfileform`      | Add file form development                | `index-main.html`                    |
| `indexAddDocket`   | Add File Docket form layout              | `index-AddDocket.html`               |
| `searchbar`        | Build the search UI                      | `search.html`                        |
| `stylecss`         | Centralized styling using CSS            | `Style-FileTracking.css`             |
| `userguide`        | Write user-facing documentation          | `docs/UserGuide.md`                  |
| `devguide`         | Developer documentation and instructions | `docs/DevGuide.md`                   |
| `changelog`        | Version tracking and release notes       | `CHANGELOG.md`                       |


## Technologies Used

- HTML5
- CSS3
- GitHub for:
  - Branching & Pull Requests
  - Issue Tracking
  - GitHub Actions (CI)
  - Project Boards
  - Releases


## File Structure

file-tracking-system/
|── src/
│ |─-index.html
| |-- login.html
| ├── index-main.html
│ |── index-AddDocket.html
| ├── Search.html
├── docs/
│ ├── UserGuide.md
│ └── DevGuide.md
├── .github/
│ └── workflows/
│ └── html-check.yml
| |__ deploy.yml
├── CHANGELOG.md
├── README.md
├── LICENSE
├── .gitignore



## Contribution Workflow

1. Each team member worked in a **feature branch**
2. After coding, they **pushed changes** to GitHub
3. They created a **Pull Request (PR)**
4. Another member reviewed and approved the PR
5. Changes were merged into the `main` branch

This workflow ensures code quality and collaboration.


## GitHub Actions

We implemented a **GitHub Actions workflow** in `.github/workflows/html-check.yml` to validate our HTML files automatically.

- It runs on every push and PR to `main`
- Uses `tidy` to lint HTML syntax
- Helps maintain clean, error-free code


## Final Notes

- Code is well-organized by feature
- Collaboration followed GitHub best practices
- All documentation and validation requirements have been met

