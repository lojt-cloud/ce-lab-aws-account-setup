# AWS Account Setup Lab - Solution

**Student Name:** [Balint Lojt]  
**Date Completed:** [06/07/2026]

---

## Exercise 1: MFA Configuration

### Screenshot:
![MFA Enabled](screenshots/mfa-enabled.png)

### Notes:
- Authenticator app used: [Google Authenticator]
- MFA setup completed successfully: [Yes / ]
- Backup codes saved: [Yes /]

---

## Exercise 2: Billing Alerts

### Screenshots:

**Billing Preferences:**
![Billing Preferences](screenshots/billing-preferences.png)

**Billing Alarm:**
![Billing Alarm](screenshots/billing-alarm.png)

**SNS Confirmation:**
![SNS Confirmed](screenshots/sns-confirmed.png)

### Configuration Details:
- Alert threshold: $[10]
- Email confirmed: [Yes / ]
- Additional thresholds created (bonus): [ No]

---

## Exercise 3: Account Alias

### Screenshot:
![Account Alias](screenshots/account-alias.png)

### Account Details:
- **Account Alias:** [balint-ironhack-bootcamp]
- **Sign-In URL:** [`https://[your-alias].signin.aws.amazon.com/console`](https://balint-ironhack-bootcamp.signin.aws.amazon.com/console)
- **Tested successfully:** [Yes]

---

## Exercise 4: Free Tier Dashboard

### Screenshot:
![Free Tier Dashboard](screenshots/free-tier-dashboard.png)

### Current Free Tier Usage Summary:

| Service | Current Usage | Free Tier Limit | Status |
|---------|--------------|-----------------|--------|
| AWS glue|    10 request| 1000000.0| ----|

### Notes:
- Any services approaching limits? [ No ]
- Any unexpected usage? [ No]

---

## Exercise 5: Reflection Questions

### 1. Why is MFA important even for a personal learning account?

**Your Answer:**
[ They can create a huge amount of bills within a short period of time using bots. Change settings/ add new users or change privileges to the account. Would give them access to the whole production lines and systems, and can pull sensitive data from there. On the company level, it would break the service level agreement and confidentiality. 

---

### 2. What would happen if you left your root user unprotected?

**Your Answer:**
Root user has unlimited access to the services, lock out, change access, and delete data.
For recovery, a password reset and if a credential key is exposed, then revoke it and create a new one immediately. Rotate the credentials with a stricter policy, audit the logs to see the damage, if there is any unusual activity or changes. Also, using dedicated storage for credentials/ secrets should be used.

---

### 3. How do billing alerts help prevent unexpected charges?

**Your Answer:**
Depending on the configuration, you get notified when you hit the selected target metrics.
Percentage-based thresholds: Getting alerts at specific milestones (e.g., 50%, 80%, and 100% of your budgeted amount) so there are no surprises.
Forecasted vs. Actual spend: Getting notified if your current usage pattern predicts you will blow past your budget by the end of the month, even if you haven't spent the money yet.
For Actions:
Optimisation is one way to go. Identifying and shutting down idle VMs, unattached storage disks, or underutilised databases.

Troubleshooting. Investigating runaway scripts, infinite code loops, or unexpected traffic spikes that are draining resources.

Automation. Setting up automated guardrails (e.g., automatically capping a service or spinning down sandbox environments when an alert fires).

Proactive monitoring helps to prevent huge end-of-the-month bills, where you can't do much about them.
Help catch early security issues, like sudden spikes(can be from leaked credentials and the attacker uses bots for crypto mining, etc).
Creates the financial accountability for the team, being able to design resource-efficient architecture from day one can save tons of money. 

---

### 4. What threshold did you set for your billing alert and why?

**Your Answer:**
10 dollar would not hurt if I reach it. For the learning stage, it is perfect, I believe, because there is real money at stake to pay attention to and can feel the weight of the mistake if it happens and learn from it faster.
Yes, I would set multiple thresholds to practise it because in a real-life environment, it is crucial to have. 

---

### 5. What is your account alias, and why did you choose it?

**Your Answer:**
- **Alias:** [balint-ironhack-bootcamp]
- **Reasoning:** [Giving it a logical, easy-to-remember name is important for future usage in case I have to work in different accounts, also for different companies ?]

---

### 6. What services are you currently using according to the Free Tier dashboard?

**Your Answer:**
[List the services you're using and their current usage levels. Are you surprised by any usage?]
AWS glue, did 10 requests so far, which is on the low side. Haven't seen any surprised usage so far. 


---

## Bonus Challenges Completed (Optional)

### Challenge 1: Multiple Billing Alert Thresholds

- [ ] $5 threshold
- [ ] $25 threshold
- [ ] $50 threshold

**Screenshots (if completed):**
[Add screenshots here]

---

### Challenge 2: CloudTrail Enabled

- [ ] CloudTrail enabled
- [ ] Logging to S3 configured

**Notes:**
[Add any notes about CloudTrail setup]

---

### Challenge 3: AWS Trusted Advisor Reviewed

- [ ] Accessed Trusted Advisor
- [ ] Reviewed recommendations

**Key recommendations found:**
[List any recommendations you found]

---

## Lessons Learned

**What was the most challenging part of this lab?**

[Your answer]

---

**What would you do differently next time?**

[Your answer]

---

**What security practices will you implement going forward?**

[Your answer]

---

## Checklist Before Submission

- [ ] All required screenshots captured and saved
- [ ] Screenshots are clear and show relevant information
- [ ] All reflection questions answered thoroughly
- [ ] Account alias documented
- [ ] Free Tier usage documented
- [ ] Work committed to Git
- [ ] Pull request created
- [ ] PR URL submitted to Student Portal

---

**Lab Completed By:** [Your Name]  
**Date:** [Date]
