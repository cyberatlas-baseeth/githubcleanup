# 🔍 GitHub Unfollow Tool

Find GitHub users who don't follow you back and unfollow them with a single click.

**No server, no installation** — just open `index.html` in your browser and go.

![Dark Theme](https://img.shields.io/badge/theme-dark-0d1117)
![No Server](https://img.shields.io/badge/server-none-success)
![License MIT](https://img.shields.io/badge/license-MIT-blue)

---

## ✨ Features

- 🔑 Authenticate with a GitHub Personal Access Token
- 📊 View follower / following / not-following-back counts
- 🔍 Search and filter users instantly
- ☑️ Select all / individual selection
- 🚀 Bulk unfollow with rate limit protection
- 📈 Progress bar and execution summary
- 🌙 GitHub-style dark theme
- 📱 Fully responsive design

---

## 🚀 How to Use

### 1. Download the Project

```bash
git clone https://github.com/cyberatlas-baseeth/githubcleanup.git
cd githubcleanup
```

Or simply download the `index.html` file directly.

### 2. Create a GitHub Token

1. [Click here to create a token](https://github.com/settings/tokens/new?scopes=user:follow&description=gh-unfollow) (GitHub token creation page)
2. Required scope: **`user:follow`**
3. Click "Generate token"
4. Copy the token

### 3. Use It

1. Open `index.html` in your browser
2. Paste your token and click **Connect**
3. Click **Load List** to fetch your followers and following
4. Select the users you want to unfollow
5. Click **Unfollow Selected**

---

## 🔒 Security

| Topic | Details |
|-------|---------|
| Token storage | Stored only in your browser's `localStorage` |
| Server communication | **Never sent to any server** — only communicates with `api.github.com` |
| Source code | Fully open and readable inside `index.html` |
| Logout | Clicking "Logout" removes the token from `localStorage` |

> ⚠️ **Important:** Never share your token with anyone. This tool uses your token solely for GitHub API requests.

---

## ⏱ GitHub API Rate Limits

- GitHub API allows **5,000 requests per hour** (authenticated)
- A **300ms delay** is applied between each unfollow request
- A warning is displayed when the rate limit drops **below 10**
- If the rate limit is exceeded, the process stops automatically

---

## 🤝 Contributing

1. Fork this repository
2. Create a new branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m 'feat: add new feature'`)
4. Push your branch (`git push origin feature/new-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
