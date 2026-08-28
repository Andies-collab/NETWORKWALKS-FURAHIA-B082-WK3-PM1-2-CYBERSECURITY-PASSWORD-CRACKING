# 🔐 1. Password Cracking with John the Ripper

Practical password-cracking exercise using **John the Ripper (JTR)** and **Johnny GUI** to recover the password of an encrypted PDF file in an authorized cybersecurity learning environment.

---

## 📌 Project Overview

This project demonstrates the use of **John the Ripper (JTR)** and **Johnny**, its graphical interface, to recover the password of a protected PDF file.

The exercise was completed as part of **Week 3 – Project Module 1** of the Networkwalks Cybersecurity Program.

The practical focused on understanding how password-protected files can be tested using password-cracking techniques and how hash values are used by password-cracking tools.

---

## 🎯 Objectives

The main objectives of this practical were to:

* Understand the basic concept of password cracking.
* Install and configure John the Ripper on Windows.
* Install and configure the Johnny graphical interface.
* Extract the hash from a protected PDF file.
* Save the extracted hash in a text file.
* Load the hash into Johnny.
* Start a password-cracking attack.
* Recover the password of the protected PDF.
* Use the recovered password to open the encrypted PDF.

---

## 🛡️ Ethical Disclaimer

This exercise was performed in an authorized cybersecurity learning environment using the provided password-protected PDF.

The techniques demonstrated in this project should only be used on files, accounts, or systems that you own or have explicit permission to test.

---

## 🛠️ Tools Used

| Tool                      | Purpose                                         |
| ------------------------- | ----------------------------------------------- |
| **John the Ripper (JTR)** | Password-cracking and password-strength testing |
| **Johnny GUI**            | Graphical interface for John the Ripper         |
| **OnlineHashCrack**       | Used to extract the hash from the protected PDF |
| **Notepad**               | Used to save the extracted hash as `hash1.txt`  |
| **Windows PC**            | Host operating system for the practical         |

---

# ⚙️ Practical Procedure

## Step 1 — Download and Install John the Ripper

John the Ripper was downloaded and installed on the Windows computer.

John the Ripper is a password-cracking tool used by security professionals to test password strength and recover passwords from supported password hashes.

The official download source provided for the practical was the Openwall website.

**Tool:** John the Ripper

**Platform:** Windows

---

## Step 2 — Install and Configure Johnny

Johnny was installed as the graphical user interface for John the Ripper.

After installation, Johnny was opened and configured to use the `john.exe` executable.

The `john.exe` file was located inside the **run** folder of the John the Ripper installation.

### Configuration

```text
Johnny GUI
     │
     └── John the Ripper
             │
             └── john.exe
```

<img width="1081" height="720" alt="location_john" src="https://github.com/user-attachments/assets/c1873b89-9405-4ba2-8227-645ff3a515de" />


---

## Step 3 — Obtain the PDF Hash

The encrypted PDF provided for the practical was used as the target file.

The PDF hash was extracted using the PDF hash extraction tool specified in the project instructions.

The extracted value was then copied for use with John the Ripper.

The expected hash format begins with:

```text
$pdf$...
```

If additional characters such as `b'` appear before the hash, they should be removed before saving the hash.

📸 **Screenshot:** PDF hash extraction result.
<img width="1346" height="741" alt="Screenshot 2026-08-28 095555" src="https://github.com/user-attachments/assets/ecdef4d2-f545-4da5-ad49-2f34754f0c51" />


---

## Step 4 — Create the Hash File

A new text file was created using Notepad.

The extracted PDF hash was pasted into the file and saved as:

```text
hash1.txt
```

The file contained the PDF hash in the format required by John the Ripper.

Example structure:

```text
$pdf$...
```

📸 **Screenshot:** `hash1.txt` containing the extracted hash.
<img width="1048" height="615" alt="hash1txt" src="https://github.com/user-attachments/assets/ff47e89a-bc8c-4417-a8af-d4abde98ceda" />


---

## Step 5 — Open the Password File in Johnny

Johnny was opened again and the **Open password file** option was selected.

The previously created:

```text
hash1.txt
```

file was selected and loaded into Johnny.

📸 **Screenshot:** `hash1.txt` loaded into Johnny.
<img width="877" height="677" alt="johhnyhash1" src="https://github.com/user-attachments/assets/b22450b3-8697-45a1-8708-dde2451138ca" />


---

## Step 6 — Start the Password-Cracking Attack

After loading the password file, **Start New Attack** was selected in Johnny.

John the Ripper then processed the PDF hash and attempted to recover the original password.

The time required for the attack depends on factors such as:

* Computer performance
* Password complexity
* Cracking method
* Hash type



---

## 🔓 Step 7 — Password Successfully Recovered

The password was successfully recovered by John the Ripper.

The recovered password was then used to open the original encrypted PDF file.

📸 **Screenshot:** Successfully recovered password.
<img width="1003" height="687" alt="crack1" src="https://github.com/user-attachments/assets/5e963b76-0a17-4672-bb3b-45b3839cb02e" />


---

## 📄 Step 8 — Open the Protected PDF

The encrypted PDF was opened using the recovered password.

The successful opening of the PDF confirmed that the password had been correctly recovered.

📸 **Screenshot:** Protected PDF successfully opened.
<img width="1216" height="629" alt="nw1" src="https://github.com/user-attachments/assets/ce986622-e9b1-404c-b346-83242f3e1407" />


The steps were repeated for all other provided encrypted PDF files.

---

# 🔄 Password Cracking Workflow

```text
              Encrypted PDF
                    │
                    ▼
             Extract PDF Hash
                    │
                    ▼
               hash1.txt
                    │
                    ▼
             Load into Johnny
                    │
                    ▼
          Start New Attack
                    │
                    ▼
          John the Ripper
                    │
                    ▼
          Password Recovered
                    │
                    ▼
             Open PDF
```

---

# 🧠 What I Learned

Through this practical exercise, I gained hands-on experience with:

* **John the Ripper**
* **Johnny GUI**
* **Password hashing**
* **PDF password protection**
* **Hash extraction**
* **Password-cracking techniques**
* **Loading hashes into JTR**
* **Password recovery**
* **Using recovered credentials to verify the result**

I also learned that password complexity has an important effect on the difficulty and time required to recover a password.

---

# ⚠️ Challenges Encountered

One challenge encountered during the practical was accessing the online PDF hash extraction website.

The website took too long to respond and could not be reached at the time. This was because of accessing Internet through Ethernet, but after switching to Wi-Fi, the website loaded successfully.

Despite the issue, the password-cracking process was successfully completed and the password was recovered.

---

# ✅ Result

The practical was successfully completed.

**Result:** ✅ Password successfully recovered

**Target:** Authorized password-protected PDF

**Tools:** John the Ripper + Johnny

**Hash File:** `hash1.txt`

**Final Verification:** Recovered password successfully opened the protected PDF.

---

# 📚 References

* **John the Ripper:** Openwall
* **Johnny GUI:** Openwall
* **Networkwalks:** Cybersecurity & Ethical Hacking Training

---


<br>

---
---

<br>

# 🔐 2. Password Cracking with Networkwalks Tools

Practical password-cracking exercise using the free, browser-based **Networkwalks Hash Calculator** and **Password Cracker** tools to recover the password of an encrypted PDF file, without installing any software.

---

## 📌 Project Overview

This project demonstrates the use of two free, in-browser tools built by Networkwalks — the **Hash Calculator** and the **Password Cracker** — to recover the password of a protected PDF file.

The exercise was completed as part of **Week 3 – Project Module 2** of the Networkwalks Cybersecurity Program.

## 📖 Background

Password cracking is the process of recovering a password from stored data or a protected file. Security professionals use it to test how strong a password is and to show why weak passwords are risky. If a password is short or common, it can be found quickly, which proves the need for strong passwords.

Many files like PDF, ZIP, and Office documents can be locked with a password. When a file is locked, its password is stored in the form of a hash. A hash is a scrambled value that represents the password. To recover the password, we first take out this hash from the file, and then run it through a cracking tool that tries different words until it finds a match.

In this lab, two free online tools made by Networkwalks were used. First, the Hash Calculator to take the hash out of a locked PDF file. Then, the Password Cracker to find the real password from that hash. Both tools run in the browser, so no installation is required.

---

## 🎯 Task

**Crack the password of the attached PDF file (`My Locked PDF1.pdf`) using the Networkwalks Hash Calculator and Password Cracker tools on a Windows laptop.**

*Note: This lab also works on Kali Linux, as both tools run in any web browser.*

---

## 🛡️ Ethical Disclaimer

This exercise was performed in an authorized cybersecurity learning environment using the provided password-protected PDF.

The techniques demonstrated in this project should only be used on files, accounts, or systems that you own or have explicit permission to test.

---

## 🛠️ Tools Used

| Tool                                | Purpose                                                         |
| ------------------------------------ | ---------------------------------------------------------------- |
| **Networkwalks Hash Calculator**     | Extracts a `pdf2john`/hashcat-compatible hash from a locked PDF |
| **Networkwalks Password Cracker**    | Runs a dictionary attack against the extracted `$pdf$` hash    |
| **Web Browser**                      | Only requirement — no local installation needed                 |

---

# ⚙️ Solution / Practical Procedure

## Step 1 — Download the Encrypted PDF

The encrypted PDF file (`My Locked PDF1.pdf`) was downloaded from the lab page:

```text
https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/
```

---

## Step 2 — Open the Networkwalks Hash Calculator

The Hash Calculator was opened in the web browser:

```text
https://networkwalks.com/hash-calculator/
```

📸 **Screenshot:** Hash Calculator landing page.

---

## Step 3 — Upload the Locked PDF

The locked PDF file was uploaded to the **PDF** tab of the Hash Calculator. The tool read the file locally (nothing uploaded to a server) and returned the crackable hash, starting with `$pdf$...`.

📸 **Screenshot:** PDF hash extraction result, with revision, version, and key-length details.

---

## Step 4 — Copy the Full Hash Value

The complete hash value was copied, starting from `$pdf$`, making sure not to miss any part of it.

📸 **Screenshot:** Copying the hash from the Hash Calculator.

---

## Step 5 — Open the Networkwalks Password Cracker

The Password Cracker was opened in the web browser:

```text
https://networkwalks.com/password-cracker/
```

This tool hashes every word in a wordlist and matches it against the PDF password hash — the same idea John the Ripper uses.

📸 **Screenshot:** Password Cracker landing page.

---

## Step 6 — Paste the Hash and Start Cracking

The `$pdf$...` hash was pasted into the Password Cracker, and the attack was started using the built-in 100-password list.

📸 **Screenshot:** Password Cracker running the dictionary attack.

---

## 🔓 Step 7 — Password Successfully Recovered

The tool tried different candidate passwords until it found a match:

```text
[-] Trying: service      ✗
[-] Trying: canada        ✗
[-] Trying: hockey        ✗
[-] Trying: killer        ✗
[-] Trying: george        ✗
[-] Trying: asdfgh        ✗
[-] Trying: zxcvbn        ✗
[-] Trying: qwertyuiop    ✗
[-] Trying: 111222        ✗
[+] MATCH: password1      ✓
```

**Recovered Password:** `password1`

📸 **Screenshot:** "Password Cracked Successfully" result screen.

---

## 📄 Step 8 — Open the Protected PDF

The locked PDF file was opened, and the recovered password was entered at the Document Open Password prompt.

📸 **Screenshot:** Entering the recovered password to unlock the PDF.

---

## Step 9 — Confirmation

The protected PDF opened successfully, confirming the password had been correctly recovered, completing the lab.
The steps were repeated for all other provided encrypted PDF files.

📸 **Screenshot:** PDF successfully opened ("Congratulations! You have captured your 1st flag.").

---

# 🔄 Password Cracking Workflow

```text
        Encrypted PDF (My Locked PDF1.pdf)
                     │
                     ▼
          Networkwalks Hash Calculator
                     │
              extracts $pdf$ hash
                     │
                     ▼
          Networkwalks Password Cracker
                     │
             dictionary attack (100 words)
                     │
                     ▼
            Password Recovered: password1
                     │
                     ▼
              Open the Locked PDF
```

---

# 🧠 What I Learned

Through this practical exercise, I gained hands-on experience with:

* **Extracting a PDF password hash without installing software**
* **The `$pdf$` hash format (used by `pdf2john` / hashcat / John the Ripper)**
* **Dictionary-attack logic** — hashing every candidate word and comparing it against the target hash
* **The difference between encryption and hashing** — encryption is reversible with the correct key, while hashing is a one-way function that scrambles plaintext into a fixed digest
* **Why weak, dictionary-based passwords are recovered almost instantly**, while long, random passwords resist cracking for much longer

---

# ⚠️ Extra Notes

* A simple 8-character password using only lowercase letters can be cracked in minutes, while a strong 12-character mixed password can take many years.
* Over 24 billion username and password pairs are available on the dark web from past breaches.
* `"123456"` and `"password"` are still among the most used passwords in the world every year.
* A 2025 leak of around 183 million Gmail login details showed how old stolen passwords keep circulating for years.

---

# ✅ Result

The practical was successfully completed.

**Result:** ✅ Password successfully recovered

**Target:** `My Locked PDF1.pdf` (authorized lab file)

**Recovered Password:** `password1`

**Tools:** Networkwalks Hash Calculator + Password Cracker

**Final Verification:** Recovered password successfully opened the protected PDF.

---

# 📚 References

* **Networkwalks Hash Calculator:** [networkwalks.com/hash-calculator](https://networkwalks.com/hash-calculator/)
* **Networkwalks Password Cracker:** [networkwalks.com/password-cracker](https://networkwalks.com/password-cracker/)
* **Networkwalks:** Cybersecurity & Ethical Hacking Training

---

## 👨‍🏫 Mentor

**Waqas Karim (CCIE)**

The practical was completed as part of the Networkwalks Cybersecurity Program under the guidance of the mentor.

---

## 👤 Author

**Furahia Mwampamba**

**Cybersecurity Program — Batch B082**

**Week 3 — Project Module 2**
