# Lab Report 4
  
  In this lab report, I will be discussing about what I did to reproduce what I did in Week 7 lab.
  
 
  The steps in the lab were as followed:
  ```
  1. Setup Delete any existing forks of the repository you have on your account
  2. Setup Fork the repository
  3. The real deal Start the timer!
  4. Log into ieng6
  5. Clone your fork of the repository from your Github account
  6. Run the test, demonstrating that they fail.
  7. Edit the code file ListExamples.java to fix the failing test (as a reminder, the error in the code is just that index1 is used instead of index2 in the final    loop in merge)
  8. Run the tests, demonstrating that they now succeed.
  9. Commit and push the resulting change to your Github account.
  ```

  ---

  **Starting from step 4.**

  I pressed the `<up>` arrow key once for the ssh command because I had already logged in previously before my wifi disconnecting once I had the command line in the terminal I pressed `<enter>`.

  
  <img width="775" alt="lab7_1" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/e60b06db-5b35-4107-b6ae-52f940748e1c">

  ---
  
  **Step 5**
  
  I then typed the command `git clone git@github.com:Rahut3/lab7.git` into the terminal to clone the repository `lab7` to my computer locally then press `<ENTER>`. Which I got from my github [website](https://github.com/Rahut3/lab7).

  <img width="579" alt="lab7_2" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/2e8e4f91-377f-42b1-8c01-c1f69419cf8f">
  
  *Note*: Since I had already done this in lab, to recreate what you would see I used the command `rm -fr lab7`. This command removes using `rm` lab7's directory and its contents recursively. `-f` means to forcefully delete them without asking permission and `r` makes it so `rm` deletes its contents and recrusively. I found this command through visiting this [website](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/delete-local-git-repository-repo-command-windows-linux-rm#:~:text=Command%20line%20Git%20repository%20delete&text=Just%20run%20the%20rm%20command,and%20folder%20to%20remain%20untouched).

  ![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/b05bcb81-1e38-4959-a968-21ecd54e2074)
  
  ---
  
  **Step 6**
  
  I then changed my directory to lab7 by typing `cd lab7`. Then I pressed `<up>` `<up>` `<up>` till I got to the command `bash test.sh` then `<ENTER>`. The result I get is the junit tester saying that there was 1 test failure.
  
  <img width="614" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/38f231ac-65b0-4623-83c1-4b0bc805b1a7">
  
  ---
  
  **Step 7** 
  
  Now to fix the mistake I first have to type the command `vim ListExamples.java` then `<ENTER>`. This is what I see after typing that in:

 <img width="600" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/9517f918-6bc2-4d81-bff3-c2e118bc4a36">

  To fix the error I need to move my cursor down to the error near the bottom. However, since we are using vim, I can't simply click on the line to move my cursor. Instead since I know I need to change the line containing the word `index1`, I type in: `/` and type in after `index1`. Then `<ENTER>` `n` `n` `n` `n` `n` `n` `n` `n` `n` `n`. `n` Means that you are moving your cursor to the next occurance of the typed in query.
  
  *Typing in `/index1` and pressing `<ENTER>`*
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/fcc54714-c790-4644-8e18-64020822a368">

  *Pressing `n` until we reach the specified location.*
  
  <img width="600" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/ffec6b5e-4678-42af-ad09-4e18b0bf84fc">

  Now that we got to where we want, then I pressed `l` `l` `l` `l` `l` to move the cursor to the left or press the `<left>` key.

<img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/c6fbc483-1526-4b10-a1b1-592827117eeb">
  
  Then I pressed `x`. `x` deletes the highlighted character.
  
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/efd28cc5-ee2a-4c78-9483-ed5d7f9c76ff">
  
  Then I pressed `i` to switch to insert mode, which allows me to edit and save changes to the file.
  
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/9978b522-6cd9-406f-acfd-b5d0b47e1926">
  
  Then I type in the number `2`.
  
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/0685fef9-43c1-454e-b9d4-5fadcaed1fd6">

  I then pressed `<ESC>` to exit out of insert mode back to normal mode.
  
  Finally I then typed the command `:wq` and `<ENTER>` to save the changes and exit out of vim.
  
 <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/d69b162e-4263-4bf0-8f64-780637d265a6">

  ---
  
  **Step 8**
  
  I then pressed `<up>` `<up>` `<up>` `<ENTER>` to enter the command `bash test.sh` (or you can manually type the command out).
  
  <img width="500" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/88530420-6866-41a5-b0bc-edd5971a530e">
  
  ---
  
  **Step 9**
  
  I then typed `git add ListExamples.java` and `<ENTER>`. This commands tells git to include the changes made to the ListExamples.java file in the next commit. Reference [website](https://www.atlassian.com/git/tutorials/saving-changes#:~:text=The%20git%20add%20command%20adds,file%20in%20the%20next%20commit.)
  
To commit I typed `git commit -m "Commit Message"` and `<ENTER>`.

  <img width="500" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/ac0905b0-3950-443a-a270-edc1fbc7834d">
  
  I then typed `git push` and `<ENTER>` to upload the changes to the remote repository.
  
  <img width="500" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/101a03e5-260e-4369-90b1-4c68449b43bb">

  




