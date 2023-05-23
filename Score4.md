  # Lab Report 4
  ---
  In this lab report, I will be discussing about what I did to reproduce what I did in Week 7 lab.
  ---

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

  I pressed the <up> arrow key once for the ssh command because I had already logged in previously before my wifi disconnecting.

  
  <img width="775" alt="lab7_1" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/e60b06db-5b35-4107-b6ae-52f940748e1c">

  ---
  
  **Step 5**
  
  I then typed the command `git clone https://github.com/ucsd-cse15l-s23/lab7` into the terminal to clone the repository `lab7` to my computer locally.
  
  <img width="579" alt="lab7_2" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/9e9e7845-d488-459d-89eb-8b252e514785">
  
  *Note*: Since I had already done this in lab, to recreate what you would see I used the command `rm -fr lab7`. This command removes using `rm` lab7's directory and its contents recursively. `-f` means to forcefully delete them without asking permission and `r` makes it so `rm` deletes its contents and recrusively. I found this command through visiting this [website](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/delete-local-git-repository-repo-command-windows-linux-rm#:~:text=Command%20line%20Git%20repository%20delete&text=Just%20run%20the%20rm%20command,and%20folder%20to%20remain%20untouched).

  ![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/b05bcb81-1e38-4959-a968-21ecd54e2074)
  
  ---
  
  **Step 6**
  
  I then changed my directory to lab7 by typing `cd lab7`. Then I pressed <up> <up> <up> till I got to the command `bash test.sh`. The result I get is the junit tester saying that there was 1 test failure.
  
  <img width="614" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/38f231ac-65b0-4623-83c1-4b0bc805b1a7">
  
  ---
  
  **Step 7** 
  
  Now to fix the mistake I first have to type the command `vim ListExamples.java`. This is what I see after typing that in:

 <img width="600" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/9517f918-6bc2-4d81-bff3-c2e118bc4a36">

  To fix the error I need to move my cursor down to the error near the bottom. However, since we are using vim, I can't simply click on the line to move my cursor. Instead since I know I need to change the line containing the word `index1`, I type in: `/` and type in after `index1`. Then `<ENTR>` `n` `n` `n` `n` `n` `n` `n` `n` `n` `n`. `n` Means that you are moving your cursor to the next occurance of the typed in query.
  
  *Typing in `/index1`*
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/fcc54714-c790-4644-8e18-64020822a368">

  *Pressing `n` until we reach the specified location.*
  
  <img width="600" alt="image" src=https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/ffec6b5e-4678-42af-ad09-4e18b0bf84fc>

  Now that we got to where we want, then I pressed `l` `l` `l` `l` `l` to move the cursor to the left or press the `<left>` key.

<img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/c6fbc483-1526-4b10-a1b1-592827117eeb">
  
  Then I pressed `x`. `x` deletes the highlighted character.
  
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/efd28cc5-ee2a-4c78-9483-ed5d7f9c76ff">
  
  Then I pressed `i` to switch to insert mode, which allows me to edit and save changes to the file.
  
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/9978b522-6cd9-406f-acfd-b5d0b47e1926">
  
  Then I type in the number 2.
  
  <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/0685fef9-43c1-454e-b9d4-5fadcaed1fd6">

  I then pressed `<ESC>` to exit out of insert mode back to normal mode.
  
  Finally I then typed the command `:wq` to save the changes and exit out of vim.
  
 <img width="400" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/d69b162e-4263-4bf0-8f64-780637d265a6">

  ---
  
  **Step 8**
  
  I then pressed `<up>` `<up>` `<up>` `<ENTR>` to enter the command `bash test.sh`
  
  <img width="500" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/88530420-6866-41a5-b0bc-edd5971a530e">
  
  ---
  
  **Step 9**
  
To commit I typed `git commit -a`

  <img width="500" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/88c5b004-41bd-4222-9889-fe23a47fe8da">
  
  Then I pressed <arrow_down> * 16 times to get to the bottom, I then pressed 'i' to insert a message for the commit.
  
  <img width="500" alt="image" src="https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/15522929-9b3b-418e-968a-db22f0b525c6">
  
  I then entered my message "This is my commit message" and I pressed `<ESC>` to exit out of insert mode. I then typed `:wq` to save the changes and exit vim. If it successful it'll return me to my command line, which it did. 
  
  Unsuccesful commits may include messages instructing what you should do next or what went wrong:

![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/59a868d4-b906-4eea-a7be-49011c8cf2c2)



