# CAPTCHA-Booster
CAPTCHA (Completely Automated Public Turing test to tell Computers and Humans Apart) is a type of automated tests that can tell human users apart from machines, aiming at filtering potential hacking into the system and maintaining the regular stability and performance of the system. It is commonly used in many Internet services and techniques to safeguard and attack CAPTCHAs have been developed. In this work, we focus on using the existing CAPTCHA datasets to iteratively generate new but difficult-to-break text-based CAPTCHAs. We first train a CNN-based breaker that can recognize the letters and digits from CAPTCHA, and then present a framework that uses the information of how the breaker solves CAPTCHAs to construct more complex CAPTCHAs. Finally, we aim to show the effectiveness of the proposed framework by counting the number of iterations needed in order to produce a robust CAPTCHA instance, and conduct an analysis on the experiment.

In this project, we aim to create:
- A CNN-based breaker that can recognize the letters and digits from CAPTCHA
- A framework that uses the information of how the breaker solves CAPTCHAs to construct more complex CAPTCHAs


Approach
We approach the problem with an iterative adversarial architecture.
Given a specific CAPTCHA dataset, we first design a <strong>CAPTCHA Breaker</strong> to attempt to recognize the given CAPTCHAs;
if the CAPTCHAs have proven breakable, we then utilize a <strong>New CAPTCHA Generator</strong> to generate more complicated CAPTCHAS.
These two steps are performed iteratively until the CAPTCHAs generated by our model is no longer breakable by the Breaker.

Read more on [my website page!](https://www.shenghui-chen.com/captcha.html)
