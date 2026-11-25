# Hi, I'm Chand

I'm learning cloud engineering by building real things on AWS and keeping all of it in code.

## What I've built

[aws-cloud-resume](https://github.com/chandakbari/aws-cloud-resume) is my CV as a serverless website. The pages live in a private S3 bucket that only CloudFront can read, and a small visitor counter runs on API Gateway, Lambda and DynamoDB. Terraform builds the whole stack with one command and tears it down with another. GitHub Actions runs the Python tests and Terraform checks on every push, then deploys the site when the frontend changes. GitHub signs in to AWS through OIDC, so there are no access keys sitting in the repo or in secrets.

You can see it live here: https://d2du93xpbftyo5.cloudfront.net

## Tools I use

AWS (S3, CloudFront, Lambda, API Gateway, DynamoDB, IAM, CloudWatch), Terraform, Python, GitHub Actions

## Next on my list

- Custom domain with Route 53 and an ACM certificate
- Remote Terraform state in S3 with locking
- `terraform plan` on every pull request
- CloudWatch alarms for Lambda errors

## Contact

[LinkedIn](https://www.linkedin.com/in/chand-akbari)
