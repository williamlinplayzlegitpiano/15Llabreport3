# CSE 15L: Servers and SSH Keys
## William Lin, 01/11/2024
---

**ChatServer Code**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/f1aa044e-d9d3-4eb9-9f76-2268010e2c9b)

---
**Example 1:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/4784f9d8-3f40-4be1-bc88-65a979413c89)

**Methods Called:**
* `main`
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
* `main`
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


