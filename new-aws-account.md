# Open your new AWS account 

Please create a new AWS Personal account. If you already have one available from work/personal that you can use feel free to use that.
If you already had a personal account that was created more than a year ago you probably already lost your free tier privileges. please create a new account with a new email address to get the free tier privileges on this new account.

### Phase 1 - Open the account
To open a new account, use these [instructions](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)

After you create your account use your promotional code and add it to your account.
You can read about adding a promo code to an AWS account [here](https://aws.amazon.com/premiumsupport/knowledge-center/add-aws-promotional-code/).

### Phase 2 - Limit root user access to your resources
Root user account credentials (the root password or root access keys) grant unlimited access to your account and its resources. It's a best practice to both secure and minimize root user access to your account.

Use the following strategies to limit root user access to your account:

- **Create an IAM** user for day-to-day access to your account. Follow the instructions [here](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-set-up.html#create-an-admin)
- Eliminate the use of root access keys
- **Use an MFA** device for the root user of your account

Read more about how to protect your account's root user [here](https://docs.aws.amazon.com/accounts/latest/reference/best-practices-root-user.html)

### Phase 3 - Activate MFA
Activating MFA can help secure your accounts and prevent unauthorized users from logging in to accounts without a security token.
For increased security, it's a best practice to configure MFA to help protect your AWS resources.

- `MFA for AWS Console` - Make sure you follow [these steps](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable.html) to activate MFA both on your root and on your user accounts
- `MFS for AWS CLI` - Follow [these instructions](https://aws.amazon.com/premiumsupport/knowledge-center/authenticate-mfa-cli/) to to enable and use MFS with your AWS CLI. 

### Phase 4 - Disable unused AWS Regions
Since we'll only be using `us-east-1` region you can disable all other regions using the AWS console. Doing so will reduce the risk of undesiered or melitous activies in these region. Use [this guide](https://docs.aws.amazon.com/general/latest/gr/rande-manage.html) to disable all but `us-east-1` region 

### Phase 5 - Monitor your account and its resources
It's a best practice to actively monitor your account and its resources to detect any unusual activity. 

Use the following strategies to monitor your account:
- Use [this guide](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html) to create a billing alarm to monitor your estimated AWS charges to receive automated notifications when your bill exceeds thresholds you define. 
