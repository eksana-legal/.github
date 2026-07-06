# .github
Organization Workflow
# 🚀 Organization Contribution Workflow Guide

Welcome to the team! To keep our main production code secure and stable on our GitHub Free plan, this organization uses a **Fork & Pull Request workflow**. 

Because your repository permissions are set to **Read**, you will not be able to push branches or merge code directly into the organization's main repositories. Instead, you will work out of your own private copy (a fork) and submit your work for review.

---

## 🛠️ The 4-Step Contribution Process

### 1. Fork the Repository
Before you write any code, you need your own sandbox copy of the repository on GitHub.
* Navigate to the organization repository you want to work on.
* In the top-right corner of the page, click the **Fork** button.
* Select your **personal GitHub account** as the owner. 
* Ensure the checkbox for **"Copy the default branch only"** is checked (unless you explicitly need other branches), then click **Create fork**.

### 2. Clone Your Fork & Make Changes
Now, pull *your* cloud copy down to your local computer to work on it. Open your terminal and run:

```bash
# 1. Clone your personal fork (replace with your username and repo name)
git clone [https://github.com/YOUR-USERNAME/YOUR-FORKED-REPO-NAME.git](https://github.com/YOUR-USERNAME/YOUR-FORKED-REPO-NAME.git)

# 2. Move into the directory
cd YOUR-FORKED-REPO-NAME

# 3. Create a new branch for your feature or bug fix (Never work directly on master/main)
git checkout -b feature/your-feature-name

# 4. Set the original Organization repo as 'upstream' (Run this once per clone)
# This lets you pull down updates made by other team members later.
git remote add upstream [https://github.com/YOUR-ORGANIZATION-NAME/YOUR-REPO-NAME.git](https://github.com/YOUR-ORGANIZATION-NAME/YOUR-REPO-NAME.git)
