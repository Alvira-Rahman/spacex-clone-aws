# SpaceX Clone — AWS S3 + CloudFront Deployment

## Live Demo
https://d2yz6zvuk5rpv2.cloudfront.net

## Project Overview
Deployed a static website on AWS using S3 for storage 
and CloudFront as a global CDN with HTTPS.

## Architecture
Browser → CloudFront (HTTPS) → S3 Static Website (HTTP)

## AWS Services Used
- Amazon S3 — static file storage and website hosting
- Amazon CloudFront — CDN, HTTPS, global edge distribution

## What I Did
- Created an S3 bucket and configured static website hosting
- Set bucket policy for public read access
- Created a CloudFront distribution pointing to S3 origin
- Configured HTTP-only origin protocol
- Verified HTTPS delivery via CloudFront domain

## Errors I Hit & Fixed
- 403 Forbidden — fixed by updating bucket policy and 
  disabling Block Public Access
- 504 Gateway Timeout — fixed by changing CloudFront 
  origin protocol from HTTPS to HTTP only

## Skills Demonstrated
AWS S3, CloudFront, CDN configuration, bucket policies, 
IAM permissions, static website hosting, HTTPS delivery
