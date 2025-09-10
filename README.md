# VCS_TB_1.0.5

---

### 🎟️ Ticket #005 – **"Clean Code, Clean Commits"**

#### 🎯 Objective:

Your engineering team is preparing the project structure and wants everything to be organized, versioned, and pushed to GitHub. You’ll split your working directory into subfolders, simulate cleaning up project files, and practice staging + committing changes *multiple times*.

---

### 📝 Tasks:

---

#### 🗂️ **1. Create Subdirectories**

Inside `project-hub/`, create **three new folders**:

* `src/` → for source code
* `config/` → for configuration files
* `logs/` → for text log files

> 🧠 These folders will keep code, configs, and logs separated and easier to manage.

---

#### 📁 **2. Move the Original Files into Their Matching Folders**

Use the `mv` command to move:

* `Main.java` → into `src/`
* `Utils.java` → into `src/`
* `application.properties` → into `config/`
* `messages.txt` → into `logs/`

🧠 *This reinforces accurate file manipulation and project organization.*

---

#### ✨ **3. Create Updated/Cleaned Versions**

Inside each new folder, create a new file named:

* `Main_refactored.java` *(in `src/`)*
* `Utils_refactored.java` *(in `src/`)*
* `application_cleaned.properties` *(in `config/`)*
* `messages_cleaned.txt` *(in `logs/`)*

These represent files that have been improved/refactored for production use.

---

#### 🛠️ **4. Begin the Git Workflow — One Folder at a Time**

Repeat the following steps **three times**, once per folder:

1. Run `git status` from the `project-hub/` root

2. Stage only the contents of **one folder** (e.g., `src/`)

3. Run `git status` again — confirm only those files are staged

4. Commit with a clear message like:

   ```bash
   Organized source code and added refactored files
   ```

5. Push the changes to GitHub:

   ```bash
   git push
   ```

6. Refresh your GitHub repo page and confirm that:

   * The folder and both files exist
   * Your commit message shows up under “Commits”

Repeat this process for:

* `config/`
* `logs/`

---

#### ❌ **5. Stage and Commit Deleted Files (Final Cleanup Step)**

At this point, the original files (`Main.java`, `Utils.java`, `application.properties`, `messages.txt`) no longer exist in the `project-hub/` root folder — but Git doesn’t know that yet!

Do the following:

1. Run:

   ```bash
   git add .
   ```

   🧠 This stages **all changes**, including deletions

2. Run:

   ```bash
   git status
   ```

   ✅ Confirm that the deleted files are staged for removal

3. Commit the cleanup:

   ```bash
   git commit -m "Removed old files from root directory"
   ```

4. Push to GitHub:

   ```bash
   git push
   ```

5. Refresh GitHub and confirm:

   * The root `project-hub/` folder no longer contains those original files
   * They now live inside their proper subdirectories

---

### ✅ Completion Checklist:

* [ ] Created `src/`, `config/`, and `logs/`
* [ ] Moved original files into the correct folders
* [ ] Created refactored/cleaned versions for each file
* [ ] Staged, committed, and pushed **one folder at a time**
* [ ] Verified each set of changes with `git status`
* [ ] GitHub repo reflects final clean structure

---
