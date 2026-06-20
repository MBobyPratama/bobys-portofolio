# Deploying your Astro Portfolio to Vercel

Vercel provides first-class support for Astro, making deployment fast, simple, and automated. Every time you push code or save changes through PagesCMS, Vercel will rebuild and update your site automatically.

---

## Prerequisites
1. A GitHub, GitLab, or Bitbucket account.
2. A free [Vercel account](https://vercel.com/signup).

---

## Step 1: Push your Code to GitHub

Ensure your project is pushed to a remote GitHub repository. If you haven't pushed it yet, run these commands in your project terminal:

```bash
git init
git add .
git commit -m "Initialize portfolio website"
# Link to your remote repository
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

---

## Step 2: Import your Project to Vercel

1. Log in to [vercel.com](https://vercel.com/).
2. On your Vercel Dashboard, click **Add New...** in the top right and select **Project**.
3. Under **Import Git Repository**, find your portfolio repository and click **Import**.

---

## Step 3: Configure and Deploy

Vercel is smart enough to detect **Astro** automatically!

1. **Framework Preset**: Verify it says **Astro** (it will auto-configure everything else).
2. **Root Directory**: Leave it as `./` (or the default).
3. **Build and Output Settings**: You can leave these minimized (default settings will use `npm run build` and target the `dist` folder, which matches your site's structure).
4. Click **Deploy**.

Vercel will start installing dependencies and building your static pages. This usually takes less than a minute.

---

## Step 4: Add a Custom Domain (Optional)

Once deployed, Vercel will provide you with a default free subdomain (e.g. `decker-theta.vercel.app`). To connect your own domain (e.g. `bobypratama.dev`):

1. Go to your project dashboard on Vercel.
2. Click the **Settings** tab.
3. Select **Domains** from the left menu.
4. Type in your custom domain name and click **Add**.
5. Follow Vercel's instructions to update your domain's DNS settings (adding an `A` record or `CNAME` record) at your domain registrar.

---

> [!TIP]
> Once both **PagesCMS** and **Vercel** are connected to the same GitHub repository, editing content inside PagesCMS will commit changes to GitHub, which will automatically trigger a new deployment on Vercel. You now have a fully functional web-based portfolio setup!
