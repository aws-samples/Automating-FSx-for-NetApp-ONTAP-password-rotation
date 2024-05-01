# Automating-FSx-for-NetApp-ONTAP-password-rotation
As part of the Well Architected Framework, it is a best practice to have a password rotation policy in place. If an administrator does not set a custom password policy, IAM user passwords must meet the default AWS password policy.

The default password policy enforces the following conditions:

- Minimum password length of 8 characters and a maximum length of 128 characters
- Minimum of three of the following mix of character types:
- uppercase, lowercase, numbers, and non-alphanumeric character (! @ # $ % ^ & * ( ) _ + - = [ ] { } | ') 
- Not be identical to your AWS account name or email address
- In the Implement a strong identity foundation pillar of the Well-architected framework, it is a best practice to rotate passwords on regular, automated frequency.

This project uses AWS Lambda and AWS Secrets Manager to manage and rotate administrative access to a FSx ONTAP filesystem.
