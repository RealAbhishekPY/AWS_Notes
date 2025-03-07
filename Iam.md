AWS IAM

IAM is the AWS Identity and Access Management Service.

IAM is used to securely control individual and group access to AWS resources.

IAM makes it easy to provide multiple users secure access to AWS resources.

IAM can be used to manage:

Users.   }   authentication
Groups.  }   authentication
Access policies.  } authorisation 
Roles.            } authorisation
User credentials.
User password policies.
Multi-factor authentication (MFA).
API keys for programmatic access (CLI).



Iam policy example 

{
“Version”: “2012–10–17”,
“Statement”: {
“Effect”: “Allow”,
“Action”: [
“iam:AddUserToGroup”,
“iam:RemoveUserFromGroup”,
“iam:GetGroup”
],
“Resource”: [
“arn:aws:iam::609103258633:group/Developers”,
“arn:aws:iam::609103258633:group/Operators”
]
}
}
