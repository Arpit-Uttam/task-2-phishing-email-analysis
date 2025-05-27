# PHISHING EMAIL ANALYSIS

I AM GOING TO ANALYZE THIS EMAIL TODAY
   
From: services@paypal-accounts.com </br>
To: [myemail@gmail.com] </br>
Subject: Urgent: Your PayPal Account Has Been Limited </br>
Date: [27 may 2025]

Dear PayPal Customer,
We regret to inform you that your PayPal account has been limited. You have 24 hours to resolve this issue, or your account will be permanently disabled.
As a result, you will temporarily lose access to PayPal features, including making purchases and sending or receiving money.
Why is my PayPal account limited?
We believe your account may be at risk due to potential unauthorized access.
How can I restore my account?
Please confirm your account information immediately by clicking the secure link below and following the instructions:

👉 [Confirm Your Information]

We appreciate your prompt attention to this matter.
Thank you for choosing PayPal.

Sincerely,
PayPal Security Team

MY FINDINGS
1. most of the phishing emails show urgency and say urgent action is required. they use dear user instead of name but official mail always contain name. so it is suspected as phishing email
2. initialy i check the sender email it look like real paypal service email so i match it with official paypal website
   this is : services@paypal-accounts.com
   original is: service@paypal.com
   ->so it is a fake or phishing mail
3. After physicaly verifying email address i go to the email header analysis i used Google email header analysis
   HEADER ANALYSIS RESULT
     -> SPF:	softfail with IP Unknown!     it fails means sender is not authorised by domain's SPF record
     -> DKIM:	 none                         it verifies mail is tempered or not it showing none means did'nt include DKIM signature
     -> DMARC: fail                         Uses SPF and DKIM to tell receiving mail servers what to do with failing messages. The email failed both SPF and DKIM, or the alignment was incorrect.
</br>
CONCLUSION:</br>
DO NOT trust this email — these results strongly suggest it’s phishing, spoofed, or fraudulent. 
   
   
    
