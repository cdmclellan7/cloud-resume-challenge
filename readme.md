# Cassandra McLellan - Cloud Resume Challenge

A work-in-progress site to host my resume on AWS. Following the steps of the [Cloud Resume Challenge](https://cloudresumechallenge.dev/docs/the-challenge/aws/).

## Progress Log

### 24 March, 2022

- Made a GitHub repo to hold the frontend static site files.
- Created a S3 bucket and configured it to host a static site. - https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html
- Made an IAM policy and user which can update the files in the S3 bucket, and added the credentials to GitHub secrets so they can be used in a GitHub Action workflow. - https://www.alexhyett.com/github-actions-deploy-to-s3
- Made a CloudFront distribution so the page can be accessed via HTTPS. - https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-https-requests-s3/ , https://aws.amazon.com/blogs/networking-and-content-delivery/amazon-s3-amazon-cloudfront-a-match-made-in-the-cloud/

### 25 March, 2022

- Added a GitHub Action that is triggered by pushes to the main branch. And runs only when files in the frontend folder are changed.
