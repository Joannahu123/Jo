---
layout: post
title: Safe computing
hide: false
---


## PII: Personally Identifiable Information  
- Information identifying a user  
- Safe computing revolves around PII: how it’s secured and how it can be exploited  

## Cookies  
- **Session**  
- **Persistent**  
- **First-party**  
- **Third-party**  

## Password Security  
- More complicated passwords = better security  

## Encryption  
- Converting data into coded format to prevent unauthorized access (**only the user can access**)  
- **Symmetric Encryption:** Same key used for encryption and decryption  
- **Asymmetric/Public Key Encryption:** More secure for internet communications  
- Encryption is used in **web security and messaging apps**  

## Phishing  
- Cyber attack where scammers trick users into giving personal info (bank details, passwords, etc.)  

### Types of Phishing  
- **Email Phishing:** Pretend to be a big company (**Check email domain**)  
- **Website Spoofing:** Attackers create fake versions of popular websites to steal login info  
  - **Avoid by typing the correct URL**  
- **Smishing:** Hackers send fake text messages pretending to be big companies and urge you to click on a link  
  - **Prevent by not clicking on links from unknown numbers**  

## Verification  
- Important for safe computing  
- Ensure everything is **legit and safe**  


## Homework hack (code)
import random
```
python
def caesar_cipher(text, shift, mode):
    result = ""
    for char in text:
        if char.isalpha():  # This part of the code only encrypts letters
            shift_amount = shift if mode == "encrypt" else -shift
            new_char = chr(((ord(char.lower()) - 97 + shift_amount) % 26) + 97)
            result += new_char.upper() if char.isupper() else new_char
        else:
            result += char  # this keeps the spaces and position unchanged
    return result

# Here is the code for getting the user input
mode = input("Do you want to encrypt or decrypt? ").strip().lower()
message = input("Enter your message: ")
shift_input = input("Enter shift value (number of places to shift, or type 'random'): ").strip().lower()

# Determine shift value
if shift_input == "random":
    shift = random.randint(1, 25)
    print(f"Random shift value chosen: {shift}")
else:
    shift = int(shift_input)

# Perform encryption/decryption
output = caesar_cipher(message, shift, mode)
print(f"Result: {output}")

```


## Completed MCQ:
<img src="{{site.baseurl}}/images/teamteach/Screenshot 2025-04-01 100640.png">