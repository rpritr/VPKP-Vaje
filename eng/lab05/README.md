# Exercise 5: Testing Password Security by Cracking Hashes

Passwords are still the most commonly used means of authentication, but they are often weak or reused. In this exercise, we will learn how a dictionary attack works on poorly chosen passwords. The purpose of this exercise is to show why it is important to use complex and long passwords.

# 🧪 Testing Password Security by Cracking Hashes

Individuals and organizations use passwords to protect access to systems, data, and services.

However, many people still use short, simple, or reused passwords, which allows attackers to quickly guess or search for matches in pre-prepared lists. Research shows that the most common passwords are still “123456,” “password,” and similar combinations, which attackers can guess in seconds.

To make storing passwords on servers more secure, hashes of passwords are stored instead of actual (plaintext) passwords. Hashing is a one-way mathematical process that calculates a shorter string of characters from a password, called a hash, from which (in theory) the original password cannot be recovered. Although hashing prevents direct theft of passwords in the event of a database breach, it does not

## 1️⃣ Introduction: Personal Identity Management

The goal is for users to learn how to:
✅ understand how password hashing works
✅ see the difference between weak and strong passwords
✅ practically use password cracking tools
✅ raise awareness of the importance of secure passwords and why we do not use weak ones

### Security of hashed values

Hashing is a one-way mathematical process that calculates a fixed-length "fingerprint" value (hash) from an arbitrarily long string of data. In information systems, it is mainly used to store password checks, since the server does not store the actual passwords, but their hash values. When the user enters a password, the system calculates its hash and compares it with the stored one.

Although hashing is an important security mechanism, it does not prevent attacks in itself. Attackers can use dictionary or brute force attacks to guess passwords and calculate their hashes until they find a match. Therefore, additional measures are crucial, such as using long and complex passwords, using a "salt" to prevent the use of pre-prepared tables (rainbow tables), and slower algorithms (e.g. bcrypt, scrypt or Argon2) to make it difficult to calculate hashes in bulk.

It is therefore important to understand that password security is not ensured by hashing alone, but by a combination of security practices: strong passwords, adding salts and using appropriate algorithms.

## 2️⃣ Activity: Using John The Ripper to Crack Hashes

### 🖥️ John The Rippper

#### Installation Instructions

1️⃣ Install John the Ripper (if not already installed):

```bash
sudo apt update
sudo apt install john
```

2️⃣ Check if you have the wordlist:

```bash
ls /usr/share/wordlists/rockyou.txt
```

If not, download it:
```bash
wget https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt
```

🔐 Data Preparation

1️⃣ Create a password.txt file with some examples:
```bash
Password1
qwerty123
My$Strong&Pass2024
letmein
Summer2024
```

2️⃣ Convert the passwords to hashes using the openssl command:

```bash
n=1; while read pass; do echo "user$n:$(echo -n "$pass" | md5sum | awk '{print $1}')"; n=$((n+1)); done < passwords.txt > hashes.txt
```

The hashes.txt file will contain the MD5 hashes:

```bash
2ac9cb7dc02b3c0083eb70898e549b63
3fc0a7acf087f549ac2b266baf94b8b1
d09b2f134b49212fb6966b5d337047e5
0d107d09f5bbe40cade3de5c71e9e9b7
e90664c0af74160644d29e4d6147969b
```

🚀 Performing the attack

1️⃣ Run the attack using a wordlist:
```bash
john --format=raw-md5 --wordlist=/usr/share/wordlists/rockyou.txt hashes.txt
```

2️⃣ Show found passwords:

```bash
john --show hashes.txt
```

### 📝 Analysis and report

- Record which passwords were found and how quickly.
- Which strong password did the program not find? Why?

## 3️⃣ Reflection and analysis

- How does the security score increase as you increase the length?
- How do special characters affect the score?
- How is a “passphrase” scored compared to a classic password?
- Which password would you recommend for everyday use and why?

## References

1. John the Ripper, *John the Ripper password cracker
*, https://www.openwall.com/john/
2. John the Ripper, GitHub, https://github.com/openwall/john
3. Rockyou.txt wordlist, https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt
4. OpenAI. (2025), *ChatGPT* (Aug 2025) [Large language model], https://chat.openai.com/