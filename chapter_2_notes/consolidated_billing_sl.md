AWS Organizations is an account management service that enables you to consolidate multiple AWS accounts into an organization that you create and centrally manage.

Can reduce overall costs.

root account with OUs under that.  A way to manage multiple account under one billing statement.  Also can create policies that get adopted by OUs.

^^^^^^^^ Not on exam ^^^^^^^^^

Consolidated Billing (on the exam)

Linked accounts to parent account.  Paying account cannot access resources of linked accounts.  Limit of 20 linked accounts.  One bill per AWS account.  Easy to track for chargeback.  Better pricing.

always enable MFA on root account
Paying account should be used for billing only.  no resources should be deployed from this account.
Billing alerts on the root account includes all linked accounts.

CloudTrail is per AWS account
    can consolidate logs using a single S3 bucket
        Turn on CloudTrail on paying account
        enable cross account
    