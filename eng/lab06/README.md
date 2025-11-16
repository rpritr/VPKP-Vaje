# Exercise 6: Personal Identity Management

In the digital world, personal identities are one of the key elements that enable our presence and operation in cyberspace. Passwords and login details are often the only barrier between our data and a potential attacker, so handling them correctly is crucial for individual security.

Unfortunately, using weak, repetitive passwords and neglecting additional security mechanisms such as two-factor authentication (MFA) is still a common practice among users, which poses a great risk.

# 🧪 Personal Identity Management

In this exercise, we will learn basic techniques for securely managing personal identities in cyberspace.

The purpose of this exercise is for students to learn basic good practices in personal identity management. In the first part, we will learn how to create complex and secure passwords and evaluate them with dedicated tools. In the second part, we will perform a practical MFA setup on popular services such as Gmail or Slack and learn how additional security steps significantly reduce the chances of a successful attack. The exercise addresses both the technical and personal aspects of responsible identity management in cyberspace.

## 1️⃣ Introduction: Personal Identity Management

The goal is for us as users to learn how to:  
✅ create secure passwords,  
✅ check their complexity and resistance to attacks,  
✅ set up two-factor authentication (MFA) to better protect our accounts.  

### Personal identities and secure passwords

Every Internet user presents their personal identity in cyberspace. This is all the data that identifies you when using online services: usernames, email addresses, passwords, security questions, profile pictures, phone numbers, even behavioral patterns.

Our identity is often scattered across many different platforms, so protecting it is challenging but extremely important. Misuse of personal identity can lead to data theft, access to bank accounts, the spread of false information in our name, or even blackmail.

The most common way to protect your identity is still passwords, which are the first line of defense against unauthorized access. Unfortunately, research shows that users often use passwords that are too short, simple character sequences, or the same passwords on multiple services. This allows attackers to quickly gain access using dictionary attacks, brute force, or already exposed databases. Therefore, passwords must be long enough, unpredictable, and consist of uppercase and lowercase letters, numbers, and special characters. It is even better if we use a different password for each service and use a password manager to help us with this.

It is also important to understand that no password is completely secure if it is not accompanied by additional security mechanisms. Therefore, whenever possible, we enable two-factor authentication (MFA), which adds another layer of protection — for example, a one-time code that we receive on our phone or generate with an application. This makes it significantly more difficult to attack an account, because the attacker also needs something that we have physically with us.

## 2️⃣ Activity: Using the Bitwarden Password Generator and Strength Evaluator

### 🔐 Password Generator

Set various parameters on the **Password Generator** page and generate one password for each setting.
Copy the passwords as you go and write them down on a sheet of paper or in a document.

### ✅ Examples to create

| Password | Length | Character set |
|------|--------------|-----------------------------------|
| G1 | 8 characters | only letters (lowercase and uppercase) |
| G2 | 12 characters | letters + numbers |
| G3 | 16 characters | letters + numbers + special characters |
| G4 | 24 characters | anything |
| G5 | Passphrase | 4 words (separated by spaces or dashes) |

Check each of the passwords above on the **Password Strength Tester** page.
For each password, write down a score:
- color indicator (e.g. red, orange, green)  
- estimated number of years to crack (if shown)  

Use a Linux tool to evaluate password strength.

Example tools:
- cracklib-check  
- pwscore 

Test passwords in Linux and compare results with Bitwarden’s website.

Calculate Shannon entropy for each password and rank them from weakest to strongest.

You can use https://timcutting.co.uk/tools/password-entropy for calculating Shannon entropy.

### 📝 Analysis and report

For each password, write down:
- The password you created.
- What settings you chose.
- Is the password safe to use and what would you change to make it even more secure?


## 3️⃣ Activity: Setting Up MFA with Bitwarden Authenticator (TOTP)

In this activity, we will learn how to enable Multi-Factor Authentication (MFA) using the Bitwarden Authenticator (TOTP — Time-based One-Time Passwords).
This is one of the most secure and practical ways to protect your online accounts.

You will enable MFA on a real service (Gmail, GitHub, Slack, Discord, etc.) and pair it with Bitwarden’s built-in authenticator to generate one-time codes.

### Example case with MFA

Pick one online service you use regularly (Gmail, GitHub, Discord). Open your account’s Security settings and set up a MFA using Bitwarden Authenticator or any other Authenticator. 

Test your MFA setup and test the login.

Write down the report with:
- Service you used
- Steps you completed
- MFA paired app

Answer questions:
- Why is TOTP more secure than SMS?
- What happens if you lose access to Bitwarden Authenticator?
- Do all services support TOTP? Why or why not?

## 3️⃣ Reflection and analysis

- How does the security score increase as you add length?
- How do special characters affect the score?
- How does a “passphrase” score compare to a classic password?
- Which password would you recommend for everyday use and why?

## References

1. OpenAI. (2025), *ChatGPT* (Aug 2025) [Large language model], https://chat.openai.com/