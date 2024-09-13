### **Git Practice Exercise**

#### **Step 1: Open Command Prompt (Windows) or Terminal (Mac/Linux)**

1. **Navigate to the Desktop:**

   - **Windows:**  
     In Command Prompt, type:
     ```bash
     cd Desktop
     ```
   - **Mac/Linux:**  
      In Terminal, type:
     ```bash
     cd ~/Desktop
     ```
     _Tip:_ `cd` stands for "change directory." This moves you to the Desktop where we will create a new folder.

2. **Create a New Folder:**
   - **Windows/Mac/Linux:**  
      In your command line, type:
     ```bash
     mkdir MyGitProject
     ```
     This creates a folder called "MyGitProject" on your desktop.

#### **Step 2: Open Visual Studio Code**

1. **Open Visual Studio Code:**

   - Open Visual Studio Code.
   - Go to **File > Open Folder**, and navigate to your Desktop.
   - Select the `MyGitProject` folder and click **Open**.

2. **Create a New File:**

   - Right-click inside the Explorer panel in Visual Studio Code (left side) and select **New File**.
   - Name the file `about_me.txt`.

3. **Add Your Information:**

   - In the `about_me.txt` file, add:
     - Your name.
     - A short summary about yourself (e.g., hobbies, interests).

4. **Save the File:**
   - Press `Ctrl + S` (Windows) or `Cmd + S` (Mac) to save the file.

#### **Step 3: Initialize Git**

1. **Check the File Path:**

   - Before proceeding with Git, make sure you're in the right folder:
     - **Windows:** In Command Prompt, type:
       ```bash
       cd
       ```
       This will show your current directory. You should see something like:
       ```bash
       C:\Users\yourusername\Desktop\MyGitProject
       ```
     - **Mac/Linux:** In Terminal, type:
       ```bash
       pwd
       ```
       This will show your current directory. You should see something like:
       ```bash
       /Users/yourusername/Desktop/MyGitProject
       ```
       If you're not in the correct folder, navigate to it by typing:
     ```bash
     cd ~/Desktop/MyGitProject
     ```

2. **Initialize Git:**

   - Run the following command to initialize Git in the project folder:
     ```bash
     git init
     ```

3. **Add the File to Staging:**

   - Use this command to add the `about_me.txt` file to Git's staging area:
     ```bash
     git add about_me.txt
     ```

4. **Commit the Changes:**
   - Commit the file with a message describing what you've done:
     ```bash
     git commit -m "Added about_me.txt with personal information"
     ```

#### **Step 4: Create a GitHub Repository**

1. **Go to GitHub:**

   - Open your web browser and go to [GitHub](https://github.com).
   - Sign in to your account or create one if you don’t have it yet.

2. **Create a New Repository:**

   - In the top-right corner of the GitHub page, click the **+** icon and select **New repository**.
   - Name the repository `MyGitProject`.
   - Keep the repository public (or private if you prefer), but **do not** check "Initialize this repository with a README."
   - Click **Create repository**.

3. **Connect Your Local Repository to GitHub:**

   - After creating the repository, GitHub will display instructions on how to connect your local repository to GitHub. You should see a section labeled **"…or push an existing repository from the command line"**.
   - Copy the following lines from the GitHub page and paste them into your terminal/command prompt:
     ```bash
     git remote add origin https://github.com/yourusername/MyGitProject.git
     git branch -M main
     git push -u origin main
     ```
   - This sets up your local repository to track changes with the remote repository on GitHub.

4. **Check Your Repository:**
   - Refresh the GitHub page, and you should now see the `about_me.txt` file in your repository.

#### **Step 5: Make Another Change**

1. **Add More Information:**

   - Go back to Visual Studio Code and open the `about_me.txt` file.
   - Add a new section describing how you got into coding.
   - Save the file by pressing `Ctrl + S` (Windows) or `Cmd + S` (Mac).

2. **Stage, Commit, and Push Again:**

   - In your terminal/command prompt, stage the file again by typing:
     ```bash
     git add about_me.txt
     ```
   - Commit the changes with a message:
     ```bash
     git commit -m "Added a section about how I got into coding"
     ```
   - Push the changes to GitHub:
     ```bash
     git push
     ```

3. **Verify on GitHub:**
   - Refresh your GitHub repository page to see the newly updated `about_me.txt` file.
