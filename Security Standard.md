# INTRODUCTION
Formally defined rules of security, technical setup and expected behaviour. Mandatory for all Keboola people, an inspiration for all our customers.

## 1ST DAY SET UP

1. You have been assigned google apps email (@keboola.com). Please log in and mind that Google G Suite Business invitations are expiring in 24 or 48 hours, jump on it ASAP.
1. Sign up for [1Password](https://keboola.1password.com/teamjoin/invitation/FU3VAJL3EJDWRCW5TH3DBBZFJU)
1. Once in 1Password, please tweak the Gmail security by turning on MFA - this is a mandatory step and has to be done right away.
1. Sign to [Global Slack](https://keboolaglobal.slack.com/signup) by email
1. Go through this "Security Guide” document and make sure everything is set up.
1. Join #Security channel on Slack and use it to ask any security-related question. If needed, promptly escalate your issue to your manager

## PRINCIPLES

### Computer:

1. Turn on hard drive encryption
    * Windows: BitLocker
    * Mac: FileVault
    * Linux: cryptmount, etc.
    * Chromebook: Check the SD card encryption
1. Strong password to your computer you [can easily remember](https://support.1password.com/strong-master-password/)
1. Windows: Use anti-virus SW (update interval not exceeding 2 days)
1. Turn on Firewall on Mac (turned off by default)
1. Install 1Password [Sign-Up Link](https://keboola.1password.com/teamjoin/invitation/FU3VAJL3EJDWRCW5TH3DBBZFJU)
1. When leaving the computer, always lock it. The screensaver can do it for you (if you set it to lock the computer on its activation). For Mac users  - there is a nice feature called Hot Corners, check it out. 
1. If something does not prevent you from it, always keep your computer up-to-date.
1. Use a separate browser for private stuff. If you are a chrome user, you can use chromium as the second one or use different browser profiles.
1. Turn off automatic saving of passwords in the browser.
1. Turn off automatic opening of downloaded files (in browser settings).
1. If you run a backup tool on your computer (time machine/windows backup, Backblaze, other offline/online tools)
    1. make sure the target is encrypted
    1. An ideal scenario is to not backup any work-related stuff and saves everything in the GDrive in the cloud. None of the files should be stored on the computer anyways.

### Mobile phone

1. Encrypted storage
    * iPhone [Data Encryption](https://ssd.eff.org/en/module/how-encrypt-your-iphone)
    * Android [Data Encryption](https://source.android.com/security/encryption/)
1. Lock your device by fingerprint or pattern, use pin as the last possibility
1. After turning the screen off, have your mobile to lock itself immediately.
1. Don't use [smart lock](https://www.digitaltrends.com/mobile/how-to-use-android-smart-lock/) trusted places (automatic login when on the location or presence of particular wifi; BT gadgets are ok if they are worn on the body (watches, etc.)
 
## BEHAVIOUR:

### Passwords

1. Do not repeat passwords, generate everything from 1Password
1. After installing 1Password, PDF with code for "[account recovery](https://support.1password.com/recovery/)" is generated
    * It is necessary not to have the PDF on a mobile phone or computer - the best solution is to print it out and have it somewhere at home. After printing it out, download the file from the computer and empty the trash bin
1. Use "[1Password Travel Mode](https://docs.google.com/document/d/10lFjHssCcwJUVOqoAzzW1WZi8MqEvPGM_DPja0gbw-Q/edit#)": you should have password connected to Keboola clients in a vault marked as Travel unsafe and set 1password to "[Travel Mode](https://support.1password.com/travel-mode/)" before departure. This will delete the Travel unsafe vaults, so if the security check makes you open your computer, they won't find the passwords in there.

### Login

1. If the service allows, always opt for 2-factor authentication [2FA](https://www.google.com/landing/2step/)
1. Use [2FA](https://docs.google.com/document/d/10lFjHssCcwJUVOqoAzzW1WZi8MqEvPGM_DPja0gbw-Q/edit#)
    1. Google G Suite requires 2FA for all accounts (new users have to activate it within 24 hours following the activation) 
    1. Always download your backup codes and save them into 1Password Secure notes (these are used instead of generated code - [google how-to](https://support.google.com/accounts/answer/1187538?co=GENIE.Platform%3DDesktop&hl=en))

### Data

1. Do not download client data into your phone
1. Avoid downloading client data into your computer if possible
1. Keep your work-related files in the cloud (Google Drive, KBC, GitHub etc.)  - if you lose your computer, the data will be preserved.

### Global Slack

Log in via Google account to Keboola Global Slack via an [automatic sign-up link](https://keboolaglobal.slack.com/signup)

#### Global Slack Rules

To prevent chaos in Channel names, follow the rules:

1. if non-keboola (@keboola.com) users are in the channel, channel name has to be prefixed by **out_**
1. temporary topics should be covered in channels prefixed by **tmp_**, channel creator is responsible for archiving channel once topic/project is closed
1. country specific topics are prefixed by region name **ca_**, **cz_**, **uk_**, **us_**
1. product specific topics are prefixed by **kbc_**

Do not disturb others 

1. automatic DnD is from 8PM to 8AM, you can customise your own settings
1. try to avoid using @everyone in General channel or @here in all other channels - mention specific users
1. employ [Slack Groups](https://get.slack.help/hc/en-us/articles/212906697-user-groups)
    1. groups can be created by Slack Admin or Slack Owner
    1. existing group can be modified by everyone, except guests


Keep discussion readable

1. always react in thread
1. check out [how thread notifications](https://get.slack.help/hc/en-us/articles/115000769927-Message-and-file-threads#catch-up-on-new-replies) are working

Message retention (required by SOC2)

1. all messages are never deleted
1. you can edit your message up to 1 hour after posting
1. messages can be deleted only Slack Admins

Invitations

1. only admins can invite others 
    1. admins are `@fisa`, `@martin.lepka`, `@pabu01` and `@marcuswong`
    1. owners are `@martin` and `@padak`
1. you can mention all slack admins by using keyword `@admins` or owners by `@owners`
1. Google auth must be used by all users except guests
1. users can't change their email address

 
## SALES / BACK OFFICE

1. Has encrypted the hard drive, uses up-to-date antivirus (update interval not exceeding 2 days)
1. Uses 1Password (and its unique generated passwords)
1. If they have work emails on their phone, they encrypt their phone as well
1. If they use mobile to log into some services, they use 1Password for phones as well
1. Updates the OS of the computer and phone regularly
1. Does not have access to clients' KBC projects
1. Never requests any sensitive data (if clients sent them to name or password for some login, they immediately ask for revoke and include an analyst in the process, who implements 1Password)

## ANALYST

1. As Salesperson/back-office  
1. Has access to KBC
    1. Uses 2FA
    1. Does not use any cloud SQL managers that remember the password for SQL workspaces ([JackDB](https://www.jackdb.com/), [Navicat Cloud](https://www.navicat.com/en/navicat-cloud), etc.)
1. Does not use API tools saving the KBC tokens to a cloud (Postman)
    1. [Paw](https://paw.cloud/) is ok, but it's necessary to have the cfg file on an encrypted drive
    1. Tips and Tricks for [Paw here](https://docs.google.com/document/d/1cixfHGJfRaJJpZMq-bAKHJLSSpSSwhMnwWrBkUluIuA/edit)
1. Never shares sensitive data via email/FB messenger etc.
    1. The password can be shared via FB messenger etc. if there is a change of password required after the first login.
1. For sharing sensitive data with a client (or the other way around) always use [1Password Guest Account](https://support.1password.com/guests-teams/) Do not use https://passion.heu.cz/ or similar for one-time password sending, since Keboola does not have visibility in the actual innards of the service
1. If some sensitive data from a client are received, they immediately ask for revoke and implement 1Password
1. When installing libraries for coding, they verify the identity of the publisher and code (e.g. public MD5 of the release, signatures etc.)
1. The Analyst always install coding tools for the user only, not for the whole system (Padak's note: in layman terms, you install without <sudo> )
1. General tips for setting up the [MAC system here](https://docs.google.com/document/d/17pn8QwkYBPgE3BwyCkawYHEgkl0j9nVkU8LNCde9k_I/edit)

## KBC TECH TEAM

1. Same as above
1. Does not use access to production infrastructure
    1. If they need to access production, they always log the reasons to Slack channel "#aws_console_login"
1. They have written confirmation for all the requests for accessing data that bypass KBC
1. Group of people with access to production infrastructure uses HW OTP like [YubiKey FIPS](https://www.yubico.com/products/yubikey-fips/) or [Ledger Nano S](https://support.ledgerwallet.com/hc/en-us/articles/115005198545-Set-up-Fido-U2F-app)
1. CloudTrail on
1. SSH keys w/ passphrase. Note: It is allowed to store passphrases in the keychain.
 
## SOCIAL HACKING

1. Never share anything with any person without proper verification
    1. Never answer questions like: "In which project is Karl active?" or "How many active users do we have?"
    1. The only exception is a Zendesk ticket created by the admin of a KBC project
    1. Exception: Zendesk ticket from a verified source
    1. A lost phone is not a reason for resetting 2FA
    1. Reset 2FA only once the proper verification took place
    1. The workaround is to invite the user with lost 2FA with another account (karl+lostphone@gmail.com)
 
## MONTHLY HEALTH CHECKS
1. Run [Windows Update](https://support.microsoft.com/en-us/help/4027667/windows-update-windows-10) / [Apple Update](https://support.apple.com/en-us/HT201222) 
1. Run antivirus update (update interval not exceeding 2 days)
1. Delete downloaded data not used in past 60 days
1. Go through and delete unnecessary logins from [1Password Watchtower](https://support.1password.com/watchtower/), perform a security check and fix any issues there

## IN CASE OF ISSUE

1. announce issue to Keboola Global Slack to #security channel
1. if not having access to Keboola Global Slack, contact your Circle Leader via phone and announce issue to support@keboola.com if possible
1. support immediately suspend your account and initiate safe-recovery
