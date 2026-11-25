# Hi, I'm Chand Akbari

Fresher looking for my first role in cloud or DevOps engineering. I'm open to graduate, junior and entry-level positions.

I learn by building. My first project puts a full AWS stack behind my own CV website, with the infrastructure written in Terraform and deployments handled by GitHub Actions.

## Skills

- Cloud: AWS (S3, CloudFront, Lambda, API Gateway, DynamoDB, IAM, CloudWatch)
- Infrastructure as Code: Terraform
- CI/CD: GitHub Actions, OIDC sign-in from GitHub to AWS
- Programming: Python, unit testing with mocked dependencies
- Web: HTML, CSS, JavaScript
- Tools: Git, GitHub, Linux shell, AWS CloudShell

## Project

### [aws-cloud-resume](https://github.com/chandakbari/aws-cloud-resume)

My CV as a serverless website, with a live visitor counter. [View the live site](https://d2du93xpbftyo5.cloudfront.net)

- Wrote the whole stack in Terraform. One command builds it and one command deletes it.
- Kept the S3 bucket private. CloudFront is the only service allowed to read it, and HTTPS is enforced.
- Built the visitor counter with API Gateway, a Python Lambda function and DynamoDB, with CORS and rate limiting on the API.
- Gave every IAM role only the permissions it needs. The Lambda can update one item in one table and nothing else.
- Set up two GitHub Actions pipelines. One runs unit tests, `terraform fmt` and `terraform validate` on every push. The other deploys the site to S3 and clears the CloudFront cache.
- Used OIDC so GitHub signs in to AWS without any stored access keys.
- Added an AWS Budget with email alerts to keep costs under control.

Tech: AWS, Terraform, Python, GitHub Actions, JavaScript

## What I'm learning now

- Custom domains with Route 53 and ACM certificates
- Remote Terraform state in S3 with locking
- Running `terraform plan` automatically on pull requests
- Monitoring and alerting with CloudWatch alarms

## Contact

I'm happy to hear about junior cloud and DevOps roles. The quickest way to reach me is [LinkedIn](https://www.linkedin.com/in/chand-akbari).
