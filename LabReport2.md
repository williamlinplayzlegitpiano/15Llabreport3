# CSE 15L: Servers and SSH Keys
## William Lin, 01/30/2024
---

**ChatServer Code**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/f1aa044e-d9d3-4eb9-9f76-2268010e2c9b)

---
**Example 1:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/4784f9d8-3f40-4be1-bc88-65a979413c89)

**Methods Called:**
* `main`: only used once when starting a server
* `handleRequest`

**Relevant Arguments:**
* URL: http://localhost:5000/add-message?s=Hello&user=jpolitz
* Extracted message (`msg`): Hello
* Extracted user (`usr`): jpolitz

**Change from Relevant Fields:**
* `chatHistory` before URL request: `""`
* `chatHistory` after URL request: `"jpolitz: Hello\n"`

**Explanation for Change:**
* Initially, `chatHistory` was empty. After processing the request, the message "Hello" from the user "jpolitz" is appended to `chatHistory`, with `\n` preparing for the next message on the next line.

---
**Example 2:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/66f8aeb1-5f3b-4949-bfb0-1bab00612409)

**Methods Called:**
* `handleRequest`

**Relevant Arguments:**
* URL: http://localhost:5000/add-message?s=Hey&user=Charlie%20Brown
* Extracted message (`msg`): Hey
* Extracted user (`usr`): Charlie Brown

**Change from Relevant Fields:**
* `chatHistory` before URL request: `"jpolitz: Hello\n"`
* `chatHistory` after URL request: `"jpolitz: Hello\nCharlie Brown: Hey\n"`

**Explanation for Change:**
* The existing `"jpolitz: Hello\n"` is appended with the message "Hey" from "Charlie Brown".

---
## SSH Keys

**Private Key**

Absolute Path: \Users\William/.ssh/id_rsa.pub

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/7355a2e2-0fae-4f27-92e3-7b577df954db)

**Public Key**

Absolute Path: /home/linux/ieng6/oce/5k/xil211/.ssh/authorized_keys

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/cca9637d-0bd0-4060-8fa8-6d25d09cb529)

**Login without Password**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/9a7f1e58-3f67-4e7f-a1ef-6de7671c3151)

---

**Something I have not Learned Before**

I have not learned anything from CSE 15L prior to taking the class. However, one thing that I was surprised the most was that we have our own ieng6 account at UCSD.
