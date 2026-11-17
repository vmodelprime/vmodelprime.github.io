# Personal Website Template (Quarto + GitHub Pages)

This template sets up a [Quarto](https://quarto.org/) personal website configured to run in **GitHub Codespaces** and deploy automatically to **GitHub Pages**.

## One-Time Setup

Follow these four steps once to launch your live website.

### 1. Create Your Repository from This Template
1. Click the green **Use this template** button at the top right of this page and select **Create a new repository**.
2. Set the **Repository name** to `<your-github-username>.github.io` (for example, if your GitHub username is `janedoe`, name your repository `janedoe.github.io`).
3. Ensure the repository is set to **Public** (required for GitHub Pages on free accounts) and click **Create repository**.

### 2. Wait for the First Build to Finish
As soon as your repository is created, GitHub automatically builds your site and saves the result to a new branch called `gh-pages`. You need this branch to exist before you can turn on Pages.
 
1. Click the **Actions** tab at the top of your repository.
2. Click the **Publish Quarto site** workflow run at the top of the list.
3. Wait for the run to show a green ✅ (this usually takes a minute or two).
> **Don't see a run?** In the **Actions** tab, click **Publish Quarto site** in the left sidebar, then **Run workflow** → **Run workflow**.
 
### 3. Turn On GitHub Pages
1. In your repository, click **Settings** in the top navigation bar.
2. In the left sidebar, click **Pages** (under *Code and automation*).
3. Under **Build and deployment**, make sure **Source** is set to **Deploy from a branch**.
4. Under **Branch**, choose `gh-pages` and leave the folder as `/ (root)`, then click **Save**.
5. Wait a minute or two, then visit `https://<your-github-username>.github.io`. Your site is live!
> **Seeing a 404 right after saving?** Give it a couple of minutes and refresh. GitHub needs a moment to publish the site for the first time.
 
---
 
## You're All Set!
 
You will **never** have to repeat the setup steps above. From this point forward, any time you commit and push edits to the `main` branch, GitHub Actions will automatically rebuild and publish your updated website.
 
> **Heads up:** The `gh-pages` branch is created and managed automatically. Don't edit it by hand. Make all your changes on `main`.