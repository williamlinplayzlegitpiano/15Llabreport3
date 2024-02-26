# Lab Report 4

## Step 4:

**log into ieng6:**
---

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/7a10a252-44ee-4899-bc26-74f9c9486872)

Keys Pressed: `ssh xil211@ieng6.ucsd.edu`

Summary: I logged into my ieng6 account.

## Step 5:

**clone:**
---

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/0e5cc96e-9b0a-4e27-943a-ab1aa9163405)

Keys Pressed: `git clone git@github.com:williamlinplayzlegitpiano/lab7.git` or `git clone <right click>` after copying ssh url

Summary: I took the forked repository and extracted the ssh url. Using that URL, I cloned the repository into my ieng6 account.

## Step 6:

**run (fail):**
---

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/f3d854d0-8336-4a20-a903-2b96015e348a)

Keys Pressed: `cd lab7`, followed by `bash test.sh`

Summary: I used `cd lab7` to change my active directory to `~/perl5/lab7`, where the directory I'm working with is located. After that, I ran `bash test.sh` to run the test scripts `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` inside the file. From the output, we can see that the test `testMerge2` under the java test file `ListExamplesTests.java` had 1 failure. 

## Step 7:

**Editing the Error**
---

Foreword: The error is located in the ListExamples.java script, on line 43. 

1. type `vim ListExamples.java` into the terminal to open the file under vim.
---





7. type `<escape>` to stop editing mode.
8. type `<:><w><q><!>` to save the changes, close the vim editor, and return to the terminal.

vim ListExamples.java, 43 down,   11 right, x, i, 2, escape, :wq!

start: 
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/74e54f5b-d224-4db7-9867-e3de4de5116d)

2. type `<4><3><down>` to go down the file 43 lines.

after 43 down:
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/79d54a0e-bcc2-4d07-9298-e91a664c16f5)

3. type `<1><1><right>` to go right the 43rd line 11 characters.
after 11 right:
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/2087d7c4-9027-4e0a-8101-6464cd7222da)

4. type `<x>` to remove the `1` from `index1`.
after x:
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/c8ac37e6-f31e-4033-8ad8-aab30aeac9a7)

5. type `<i>` to insert the new missing value after `index`.
after i:
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/161e25a2-962e-42b2-aa30-019640299a7f)

6. type `<2>` to insert `<2>` after `<index>` for `<index2>`.
after 2:
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/e686747d-717b-425c-b8fe-b66dd807dd85)

## Step 8:

run (pass):
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/dd6d3812-9cad-4f29-ab08-f4e790b1359f)

## Step 9:

add, commit, push:
![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/8dea82c4-c73a-4755-a369-c3d1cc131eef)
