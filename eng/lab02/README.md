# Exercise 2: OSINT – collecting information about individuals online

Open Source Intelligence (OSINT) is information sources that are publicly available, for example: websites, social networks, forums, search engines. In this exercise, we will look at how even the average Internet user can access another person's personal information if it is not properly protected.

# 🧪 Basics of OSINT

OSINT represents intelligence from open sources, and as a technique it represents the collection and analysis of information that is publicly available through open and legal sources.

OSINT is based on the principle that a huge amount of data can be found on the Internet and other public media that can be used for various purposes – from cybersecurity, ethical hacking, to journalism, research and security investigations.

## 1️⃣ Introduction: Collecting information about individuals online

The objectives of the exercise are:  
✅ Learn about OSINT techniques for collecting publicly available information about individuals.  
✅ Awareness of how much personal data can be found online.  
✅ Discussion on how to protect ourselves from overexposure.  

### Tools for collecting information about individuals

Sherlock is an OSINT tool that searches for usernames on over 300 social networks and online platforms. It allows you to enter a username as a string, and the tool checks if there are profiles with that name on known websites.

![Sherlock example](https://github.com/sherlock-project/sherlock/raw/master/docs/images/demo.png)

[Documentation and GitHub](https://github.com/sherlock-project/sherlock)

Maigret goes one step further than Sherlock, as in addition to searching for usernames, it offers a detailed analysis of an individual's digital footprint, including additional metadata and often also the activity of user accounts.

[Documentation and GitHub](https://github.com/soxoj/maigret)

## 2️⃣ Activity: OSINT - Collecting information about an individual

Choose a public figure (e.g. a famous journalist, politician, athlete) or a fictitious person with pre-prepared data for training (it is recommended to use anonymized data to respect privacy).

### 🖥️ Sherlock

🔷 1️⃣ Environment preparation

Sherlock is a tool that runs in a shell with Python installed.

✅ If you work in a Linux environment (e.g. Kali), Sherlock is often already installed or install it:

```bash
git clone https://github.com/sherlock-project/sherlock.git
cd sherlock
pip3 install -r requirements.txt
```

Run Sherlock:

```bash
python3 sherlock <username>
```

### 🖥️ Maigret

🔷 2️⃣ Alternative or supplement to Sherlock

Maigret, like Sherlock, runs in a shell with Python installed. It also supports a web interface and various output and report formats.

✅ Installing Maigret (if not already installed):
```bash
pip install maigret
```
or from the source code:

```bash
git clone https://github.com/soxoj/maigret.git
cd maigret
pip install -r requirements.txt
```

On Kali Linux:
```bash
python3 -m venv venv
source venv/bin/activate
pip install .
```
Launching Maigret:

```bash
maigret <username>
```

🔷 Comparing tools
Use both programs for the same username and compare the results: which tool found more profiles? Which gives more transparent data?

Think about it: were there profiles found on social networks where you didn't expect them?

### 📝 Analysis and Report

- Compare the results of Sherlock and Maigret. What differences did you notice?
- Did you find any sensitive information (e.g. email address, private pictures, phone number)? How could the person protect it from being publicly available?

## 3️⃣ Reflection and Analysis

- What information was the easiest to find? What was the hardest to find?
- How would you adjust your own online behavior after doing this exercise?
- Do you think the use of OSINT tools is ethically questionable? In which cases is it justified?

## References

1. Sherlock Project, *Sherlock: Find usernames across social networks*, GitHub, https://github.com/sherlock-project/sherlock
2. Maigret, *Maigret*, GitHub, https://github.com/soxoj/maigret
3. OSINT Framework, *OSINT tools and resources collection*, https://osintframework.com/
4. OpenAI, (2025), *ChatGPT* (Aug 2025) [Large language model], https://chat.openai.com/