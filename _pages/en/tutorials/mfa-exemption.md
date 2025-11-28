---
title: Exempted Multi-Factor Authentication Setup
altLangPrefix: tutoriels/exemption-amf
description: How to get connected to LaunchPad AWS
tags: [mfa, security]
#draft: false
last_updated: 2025-11-28T21:49:56Z
---

### Introduction
<div class="alert alert-warning">
	<p>This page is <b>only</b> for persons who have been given an exemption by our team regarding MFA for approved reasons.</p>
</div>

<div class="alert alert-warning">
	<p>The <b>SMS</b> option is currently available when given an MFA exemption but it will be deprecated soon as it is insecure so we recommend using TOTP (follow this page's instructions) authentication.</p>
</div>

This page is set up so you can follow instructions on how to properly set up TOTP ([Time Based One Time Password](https://en.wikipedia.org/wiki/Time-based_one-time_password)) when an exemption was given so a less secure than push authentication method can be used. This exemption is given under special circumstances and is decided by our team. Please discuss with us before trying to follow these instructions.

#### Instructions

- When login in for the first time on our environment with the exemption set on your account, you will be asked to set up MFA and will have many options. Select the "Microsoft Authenticator" option.  
![](/assets/images/en_sign_in_methods.png)

- Then, click on "I want to use a different authenticator app," this option is only truly available when you are in our exemption list.  
![](/assets/images/en_use_different_app.png)

- Follow the instructions to set up a new account in your authenticator application (you can use any TOTP enabled authenticator app like Google Authenticator for example)

- Scan the given QR code in your authentication app.  
![](/assets/images/en_auth_qr_code.png)

- Enter the 6 digit code given by your authenticator app.

- Your authenticator app should be configured and working now.

#### Recommended TOTP applications

- Google authenticator 
- Proton authenticator
- LastPass Authenticator
- You can technically use any authenticator apps
