# Technical Design

## Phase 1: Automate the creation of a new static website.

1. Create an S3 bucket with the appropriate policy.
2. Create a CloudFront distribution to serve content from this S3 origin.
3. Generate a wildcard SSL certificate in ACM for the domain. Output the TXT record values needed in DNS for approval.
4. Manually create the Route 53 CNAME record for the hosted zone to point to the CloudFront distribution.
5. Upload a placeholder index.html file to the S3 bucket for testing.

## Phase 2: Automate the deployment of content to the website.

## Phae 3: Create a CMS to allow content creation and publishing.
