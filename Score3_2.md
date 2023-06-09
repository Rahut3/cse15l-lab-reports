# Lab Report 3
---

In this lab report, I am writing about the command `grep` in bash. Below are 4 interesting command-line options for the `grep` command.

---

The first command I am showcasing is `grep -o "search term" *.txt | wc -l`. 

In this example below my current directory is `/Users/rahut/Documents/GitHub/docsearch/technical/biomed`. This command searches for the inputed "search term" and it counts the search term words in the file directory. Using `grep -o`, `grep` searches the given files for lines that match the search query, the `-o` makes it so grep prints out each occurence of the search term instead of the whole line. The pipe `|` character acts like `>` symbol in bash but instead it uses the grep output as an input for the `wc` command. `wc -l` Is used to count the lines of the grep output. This is useful to find how many instance of the word each lines contains.

![img1](labss1.png)

This next example shows me using it to find how many occurences each lines contains the word "bar" in txts files in the 911 report directory.

![img2](lab3ss2.png)

---

The second command I am showcasing is `grep -A # "word" FILE`. The -A in the command is used to specify how many lines to print after the line containing "word". This can be adjusted by changing the #. This can be useful by to get a brief description, or a lines of code that contains an error. It can also be used to see what lines of the word have after the Below are two examples on me using the command. Both with varying #s.

![img3](lab3ss3.png)

![img4](lab3ss4.png)

---

The third command I am showcasing is `grep -r "word" FILE`. This is similiar to the first command but now instead counting the words in a line, it showcases the line that the word is contained in. This can be useful if you want to find a line that contains that word and in which file it is in. You can use * instead of a specific file to print out all the lines that containst that word in the directory. It'll show you the line as well as the txt file.

![img5](lab3ss5.png)

![img6](lab3ss6.png)

---

The fourth and last command I am showcasing is `grep -v "word" FILE`. This command shows all the lines that doesn't contain the given "word" in a given file. `-v` basically inverts the match, therefore showcasing lines that don't match with the "word". This is useful if you want to find all the lines that doesn't contain a give "word". 

![img7](lab3ss7.png)

This example below utilizes `[ ]` meaning any character inside will be counted as indiviual characters rather than one word.

![img8](lab3ss8.png)


Credits:

First 2 examples I had gotten from asking Chat gpt. The third and fourth examples I had gotten from [here](https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/). I also asked Chat GPT in some explaintions of what certain syntax did.
