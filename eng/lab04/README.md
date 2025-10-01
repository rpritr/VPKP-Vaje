# Exercise 4: Social Engineering and Defenses

Social engineering exploits human psychology, not technical vulnerabilities.

Attackers target the emotions, habits, and inattention of individuals to gain access to information or systems without using complex hacking techniques.

# 🧪 Exercise 1: Let's get to know cyberspace

In the first exercise, we learned how much information individuals share in cyberspace — now let's look at how this information can be misused.

We will learn about the most common social engineering methods, such as phishing, vishing, pretexting, and baiting, and how to recognize and effectively protect against them.

Around 90% of attacks on individuals occur precisely because of poor awareness and exploitation of social engineering — this exercise builds a bridge between theory and everyday practice, which we will need in both our private and professional lives.

The second exercise is about learning about social engineering:

- What is social engineering?
- What are the techniques of social engineering and how do we detect it?
- How can we protect ourselves from social engineering?

## 1️⃣ Introduction: Social engineering techniques

Exercise objectives:
✅ Identify the main social engineering techniques.
✅ Check your own preparedness for such attacks.
✅ Learn about specific defense strategies and good practices.

### Identifying social engineering techniques

📧 Phishing

The most common form of attack: the attacker sends an email pretending to come from a trusted organization and thus convinces the user to click on a link or provide certain information.

Example:

"Your account will be deactivated if you do not update your information. Click here to log in."

🛑 What to look out for: incorrect email addresses, grammatical errors, suspicious URLs.

🎯 Spear Phishing

A targeted attack on an individual, often tailored to their details (e.g. job title or past communication).

Example:

“Hello, John. As agreed last week, I am sending you documents. Please open the attachment.”

☎️ Vishing (Voice Phishing)

The attacker calls the victim and presents himself as an official (e.g. technical support, bank) and requests information.

Example:

“This is from the bank. We need your PIN to unblock your account.”

📝 Pretexting

The attacker makes up a story (pretext) to obtain information or access. This technique is based on establishing trust.

Example:

“I am a new employee in IT support. I need your user account to check the system settings.”

🎁 Baiting

The attacker offers a tempting “bait” to the victim to install the malware themselves.

Example:

A USB stick labeled “Confidential” or “Payment Details” left in a company parking lot.

🎯 How to recognize them?

✅ Always verify the identity of the sender/caller.
✅ Don’t click on suspicious links or open unknown attachments.
✅ Don’t share personal or login information over the phone or email.
✅ If a story seems suspicious or too urgent — check with an official source.

## 2️⃣ Activity: Phishing Case Analysis

### Package Pickup Email

From: dostava@postapaket.xyz
Subject: Your package is awaiting delivery!

Dear,

We would like to inform you that your package is awaiting delivery. To pick up, you must confirm your details within the next 24 hours, otherwise the package will be returned to the sender.

Click here: http://posta-dostava-verify.paket-secure.ru

For assistance, please contact our support.

Thank you,
Posta Team

### Account Deactivation Email

From: varnost@bankaa-si.com
Subject: Your account will be deactivated!

Dear user,

We have detected suspicious activity on your bank account. If you do not confirm your details within the next 12 hours, we will be forced to deactivate your account.

Click here to confirm: http://bankaa-si-login.net

Thank you for your cooperation.

Bank Security Service

### Prize Email

From: nagrade@promocije.win
Subject: Congratulations! You have won a prize!

Dear!

You have been drawn as the winner of the main prize in our promotion! To claim your prize, please enter your details and pay a symbolic delivery fee.

Click here: http://promo-claim-now.biz

We look forward to your participation!

Promotion Team

### Google Phishing Test

Test your knowledge of phishing emails with the help of the Google Quiz: https://phishingquiz.withgoogle.com/

## 3️⃣ Activity: Checking phishing emails

Every email has a header that contains technical information about the sender, recipient, time, IPs and servers. The header is important for investigating suspicious emails.

Examples of suspicious signs:
- Different “From” and “Return-Path”
- IPs from strange countries
- Mismatched sender domain
- SPF/DKIM/DMARC errors

Write a short report:
- What is the actual IP of the sender?
- Does the sender domain match the “From” address?
- What country does the message roughly originate from?
- Are there any signs of redirection through multiple servers in the header?
- Are there SPF/DKIM/DMARC errors?

In your email client, try to find a message in the SPAM folder that you suspect could be a phishing message and analyze it. Write down the results.

## 4️⃣ Reflection and analysis

- How quickly do you notice the suspiciousness of a phishing message?
- Would you recognize this message as dangerous without the header?
- What advice would you give to someone who is new to email regarding the dangers lurking in terms of social engineering?



## References

1. OpenAI. (2025), *ChatGPT* (Aug 2025) [Large language model], https://chat.openai.com/