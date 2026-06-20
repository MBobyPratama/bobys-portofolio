# PagesCMS Tutorial Guide

[PagesCMS](https://pagescms.org/) is a user-friendly, open-source Content Management System (CMS) designed for static site generators like Astro. It reads the files in your Git repository and provides a clean, visual interface to edit them.

Your repository is already pre-configured with a [.pages.yml](file:///C:/Users/bobyj/Documents/Kuliah/project/portofolio/decker/.pages.yml) file that maps all your portfolio fields (Projects, Experience, Education, Certifications, and Blog) directly into PagesCMS.

---

## Step 1: Connect your Repository to PagesCMS

Before logging in, make sure your local codebase is committed and pushed to your git hosting provider (e.g. GitHub).

1. Go to [pagescms.org](https://pagescms.org/).
2. Click **Start editing** or **Login with GitHub** (or GitLab).
3. Authorize PagesCMS to access your repositories.
4. Select your portfolio repository from the list (e.g. `decker`).

---

## Step 2: Navigate the CMS Interface

Once loaded, you will see a clean dashboard:
* **Sidebar**: Located on the left side, it lists the collections defined in your `.pages.yml`:
  * **Projects** (Collection of Markdown files)
  * **Education** (YAML file list)
  * **Certifications** (YAML file list)
  * **Experience** (YAML file list)
  * **Blog** (Collection of Markdown files)
* **Main Area**: Displays the list of entries for the selected collection.

---

## Step 3: Edit Existing Content

1. Click on any section in the sidebar, such as **Experience** or **Projects**.
2. Click on the item you want to edit.
3. Modify the fields:
   * **Text boxes**: Simple strings like dates, titles, and schools.
   * **Select menus**: Multi-select dropdown tools (e.g., PHP, Laravel, Tailwind) which we configured in `.pages.yml`.
   * **Markdown/Rich Text**: For blog contents or descriptions.
4. Click **Save** (this will automatically commit and push the changes directly to your GitHub repository, which triggers your deployment platform to rebuild your site).

---

## Step 4: Add New Entries

### For Collection Items (Projects & Blog)
1. Click **Projects** or **Blog** in the sidebar.
2. Click the **Create New** (or **+**) button at the top right.
3. Fill in the required metadata (ID, title, tools used, description, etc.).
4. Save the file. PagesCMS will create a new `.md` file inside `src/content/projects/` or `src/content/blog/` automatically.

### For List Items (Experience, Education, Certifications)
1. Click **Experience**, **Education**, or **Certifications** in the sidebar.
2. Scroll to the bottom of the list.
3. Click **Add item** (or equivalent list-addition buttons).
4. Fill in the fields for your new position or certificate.
5. Click **Save**.

---

## Step 5: Uploading Media

1. In any collection supporting media (or in markdown content editors), select the media/image upload field.
2. Upload your profile picture or project screenshot.
3. PagesCMS will automatically store the files in your `src/assets` directory, keeping your repository organized.

---

> [!NOTE]
> Since PagesCMS modifies standard files on your Git repository, you can always choose to bypass the web interface and edit the YAML/Markdown files directly inside the [src/content/](file:///C:/Users/bobyj/Documents/Kuliah/project/portofolio/decker/src/content/) directory using your code editor.
