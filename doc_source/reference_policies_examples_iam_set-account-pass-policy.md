# IAM: Allows Setting the Account Password Requirements Programmatically and in the Console<a name="reference_policies_examples_iam_set-account-pass-policy"></a>

This example shows how you might create a policy that allows a user to view and update their account's password requirements\. The password requirements specify the complexity requirements and mandatory rotation periods for the account members' passwords\. This policy also grants the necessary permissions to complete this action on the console\.

To learn how to set the account password requirements policy for your account, see [Setting an Account Password Policy for IAM Users](id_credentials_passwords_account-policy.md)\.

```
{
    "Version": "2012-10-17",
    "Statement": {
        "Effect": "Allow",
        "Action": [
            "iam:GetAccountPasswordPolicy",
            "iam:UpdateAccountPasswordPolicy"
        ],
        "Resource": "*"
    }
}
```