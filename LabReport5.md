# Lab Report 5

## Part 1: Debugging Scenario

### Student's Post

---

**Code:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/9b503219-1946-4f11-b921-5a16999665af)

**Output:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/42a419b4-b5d5-4db9-ac71-2444b83bea9c)

**Problem Description:**

Hey everyone, I'm having trouble with my Java program. I'm trying to run it, but it's giving me this weird error message. The error message says something about an `ArrayIndexOutOfBoundsException`. I think it might be related to how I'm accessing elements in my array, but I'm not sure. Can anyone help me figure out what's going wrong?

### TA's Response

---

Hi there! Thanks for reaching out. It looks like you're encountering an `ArrayIndexOutOfBoundsException`, which typically occurs when you're trying to access an index in an array that doesn't exist. Please check your `for` loop. How many times would the `for` loop run and how many indexes are in your `numbers` array? 



### Student's Response

---

**Fixed Code:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/f60ed29f-73fb-443d-9ecd-f689183432ab)

**Fixed Output:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/05a78bc3-e16a-4501-84e4-7043e92549da)

**Response:**

Thanks for the help. I realized that the `i <= numbers.length` would loop the `for` loop 6 times when the `numbers` array was 5 indexes long. I believe this resulted in the `for` loop to access an index that did not exist. After changing to `i < numbers.length`, my output no longer had the `ArrayIndexOutOfBoundsException` error, ultimately fixing my bug.

### Setup Information

#### **File Directory and Structure**

**Path `pwd`:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/6bc5ac6a-56b9-49ac-a6eb-8335dd75bfef)

**File Directory `ls`:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/6044763f-56f4-4ac4-9181-5499c3f3b9f8)

**Contents of Each File Before Fixing Bug:**

`Main.java`:

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/9b503219-1946-4f11-b921-5a16999665af)

`test.sh`:

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/ee8d8a2d-8f01-4ce8-8727-3d4b2f799f57)

**Full Command Line to Trigger the Bug**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/ff445dbd-a82a-4884-8ddb-3d332b699bef)

**Description of What to Edit to Fix Bug**

To fix this bug, the user must make sure the number of times the loop is run is **equal** to the size of the respective array. In this scenario, because the size of `numbers` array is 5, the `for` loop condition `i <= numbers.length` needs to change to `i < numbers.length` to decrease the number of times looped from 6 to 5.



