# Cyber-Security-Internship---Task-2
# 📧 Phishing Email Analysis Task

## 🎯 Objective
Analyze a phishing email sample and identify key phishing characteristics.

## 🔍 Phishing Email Analysis Report

### 📌 Email Subject: "Urgent: Your Account Has Been Suspended!"

### 📤 Sender Address: `support@netflix-support.com`

---

### ⚠️ Phishing Indicators Found

#### 1. Spoofed Sender Address
- Appears as: `support@netflix-support.com`
- Actual Netflix domain is `@netflix.com`, so this is **fake and misleading**.
- Trick: Adding a hyphen (`-support`) to seem legitimate.

#### 2. Header Discrepancies
- Return-Path: `bounce@abc.ru` (suspicious foreign domain)
- SPF/DKIM checks **failed** in header analysis.
- Origin IP located in **Russia**, unrelated to Netflix.

#### 3. Suspicious Links
- Visible link: `https://netflix.com/verify`
- Actual link (on hover): `http://netflix-login-security-update.xyz`
- Link leads to **phishing site** disguised as a login page.

#### 4. Urgent Language
- Body content example:
  > “Your Netflix account has been suspended. Immediate verification required or your account will be deleted within 24 hours.”
- **Scare tactic** to force quick action.

#### 5. Spelling & Grammar Errors
- Found multiple issues:
  - "verificaiton" instead of “verification”
  - "you’re account will be delete"

#### 6. Fake Branding
- Netflix logo embedded, but image hosted on an external server `img001.evilcdn.net`.
- No personalization (e.g., "Dear User" instead of user's name)

#### 7. Attachment
- Attached file: `Netflix_Update.pdf.exe`
- PDF and `.exe` combined — classic malware delivery trick.
- Antivirus flagged it as malicious.

---

### 🧾 Summary of Phishing Traits

| Trait                            | Found |
|----------------------------------|:-----:|
| Spoofed sender email             | ✅    |
| Failed authentication (SPF/DKIM) | ✅    |
| Mismatched URLs                  | ✅    |
| Threatening/Urgent language      | ✅    |
| Grammar/spelling issues          | ✅    |
| Suspicious attachment            | ✅    |
| Generic greeting (no name)       | ✅    |

---

### ✅ Conclusion

This email is a **phishing attempt** designed to trick users into providing login credentials or installing malware. Users must:
- Never click on unknown links.
- Always verify sender email domains.
- Use a secure browser and email scanner.

---

## ✅ Outcome
Improved awareness of phishing tactics and enhanced ability to analyze email threats.

