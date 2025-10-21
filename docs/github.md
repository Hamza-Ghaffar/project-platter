# 🧰 GitHub Integration

Project Platter can create a GitHub repository via API during project setup.

---

## 🔑 Requirements

- GitHub username
- Personal Access Token (PAT)

### Recommended PAT Type
Use a **Classic Personal Access Token** with:
- `repo` (for private repos)
- `public_repo` (for public repos)

> ⚠️ Fine-grained tokens often fail for repo creation.

---

## 🧩 Process Flow

1. Prompts for username, token, and repo visibility  
2. Sends POST request to `https://api.github.com/user/repos`  
3. On success, clones URL and configures remote  
4. Pushes commits and branches if requested


