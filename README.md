# GitHub Assignment

This assignment will guide you through the basic steps of using GitHub to create and manage your code repositories.

## Creating a Local Repository

1. **Create a Directory:**
   - Create a new directory for your project using the following command:
     ```bash
     mkdir folder1
     ```
     Replace `folder1` with the desired name of your project directory.

2. **Initialize a Git Repository:**
   - Navigate into the newly created directory:
     ```bash
     cd folder1
     ```
   - Initialize a Git repository using the following command:
     ```bash
     git init
     ```

## Making Changes and Committing

1. **Create a File:**
   - Create a new file within your project directory using the following command:
     ```bash
     touch <file_name>
     
     Replace `<file_name>` with the desired name of your file.

2. **Stage Changes:**
   - Mark all changes made to the files in your project directory for tracking using the following command:
     bash
     git add .
     ```
     The `.` symbol indicates all files in the current directory.

3. **Commit Changes:**
   - Commit the staged changes with a descriptive message using the following command:
     ```bash
     git commit -m"new file added"
     ```
     Replace the message with a more specific description of the changes you made.

## Linking to a Remote Repository

1. **Set Default Branch:**
   - Set the default branch for your local repository to `main` using the following command:
     ```bash
     git branch -M main
     ```

2. **Add Remote Repository:**
   - Connect your local repository to a remote GitHub repository using the following command:
     ```bash
     git remote add origin <url>
     ```
     Replace `<url>` with the HTTPS URL of your remote GitHub repository.

## Pushing Code

1. **Push Code to Remote Repository:**
   - Push the local repository's contents to the remote repository using the following command:
     ```bash
     git push origin main
     ```
   - This will push your local changes to the remote repository, making them accessible online.



# PULLING

## Scenario: Two Machines

**Machine 1** and **Machine 2** both have a clone of the same GitHub repository.

### Making Changes on Machine 1

1. **Clone the Repository:**
   - Clone the GitHub repository to your local machine using the following command:
     ```bash
     git clone <url>
     
     Replace `<url>` with the HTTPS URL of your remote GitHub repository. This will create a copy of the repository on your local machine.

2. **Change Directory:**
   - Navigate into the newly created directory:
     bash
     cd <dir_name>
     ```
     Replace `<dir_name>` with the name of the directory created by the cloning process.

3. **Create a File:**
   - Create a new file within the project directory using the following command:
     ```bash
     touch <file_name_1>
     
     Replace `<file_name_1>` with the desired name of your file.

4. **Stage Changes:**
   - Mark all changes made to the files in your project directory for tracking using the following command:
     bash
     git add .
     ```
     The `.` symbol indicates all files in the current directory.

5. **Commit Changes:**
   - Commit the staged changes with a descriptive message using the following command:
     ```bash
     git commit -m"hello"
     ```
     Replace the message with a more specific description of the changes you made.

6. **Set Default Branch:**
   - Set the default branch for your local repository to `main` using the following command:
     ```bash
     git branch -M main
     ```

7. **Push Changes:**
   - Push the local repository's contents to the remote repository using the following command:
     ```bash
     git push origin main
     ```
     This will push your local changes to the remote repository, making them accessible online.

### Attempting to Push on Machine 2

1. **Try to Push Changes:**
   - Attempt to push your local changes to the remote repository using the following command:
     ```bash
     git push origin main
     
     This will result in an error message because your local repository is out of date with the remote repository.

### Updating the Local Repository on Machine 2

1. **Pull Changes:**
   - Synchronize your local repository with the remote repository to get the latest changes using the following command:
     ```bash
     git pull origin main
     ```
     This will merge the changes from the remote repository into your local repository.

2. **Verify Updated Repository:**
   - Check the contents of your local repository to confirm that the changes from Machine 1 are now present:
     ```bash
     ls
     ```
     This will list the files in your local repository, which should now include both `<file_name_1>` and `<file_name_2>`.

3.  **Push Changes:**
   - Push the local repository's contents to the remote repository using the following command:
     ```bash
     git push origin main
     ```
     This will push your local changes to the remote repository, making them accessible online.
