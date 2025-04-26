🌎 Static Website Deployment with S3 + Cloudflare + GitHub Actions
This project demonstrates how to host and auto-deploy a static website using AWS S3, Cloudflare, and GitHub Actions, ensuring global delivery with HTTPS security.

📚 Project Overview
-->Host a static HTML/CSS site on AWS S3 (Free Tier).
-->Connect it to Cloudflare for CDN and SSL.
-->Set up GitHub Actions for automatic deployment on code push.

🛠️ Tools and Technologies
* AWS S3 – Static website hosting.
* Cloudflare – DNS management, CDN, and SSL/TLS.
* GitHub Actions – CI/CD workflow.
* HTML/CSS – Static content.

🚀 Deployment Steps
1. Create Static Site
Simple HTML and CSS page prepared.

2. S3 Bucket Setup
Created a new S3 bucket.
Enabled static website hosting.
Configured public read permissions.

3. GitHub Actions Workflow
Added a .github/workflows/deploy.yml file:
Trigger: on: push
Action: aws s3 sync static files to the S3 bucket.

4. Cloudflare Configuration
Domain DNS managed via Cloudflare.
SSL/TLS set to Full (Strict) mode.
Caching and optimization rules applied.

5. Validation
Confirmed automatic deployment via GitHub Actions.
Verified live site accessibility with HTTPS.

📸 Screenshots
Live Website , GitHub Actions CI/CD , CloudFlare
![bucket](https://github.com/user-attachments/assets/a8b8147a-830b-42ca-a6bc-cffeae0059df)
![Bucket website hosting](https://github.com/user-attachments/assets/bf4806da-49bd-4f2a-bcdc-b39bdc303ac0)
![github actions](https://github.com/user-attachments/assets/84691d68-3b88-45de-82bf-ad5317248d06)
![cloudflare workers](https://github.com/user-attachments/assets/41b64fe2-7284-4003-b4d7-843c9f3d50ed)
![deploy](https://github.com/user-attachments/assets/5386ef96-7f09-454e-8589-8c2f14d2ce5c)
![live website](https://github.com/user-attachments/assets/9c40ff27-d927-4815-8c18-714dd57ad0f0)

🔗 Live Website
👉 https://workers-playground-frosty-glade-f8c7.soneeyasubramanian.workers.dev/

📂 Repository Structure
.
├── index.html
├── styles.css
└── .github/
    └── workflows/
        └── deploy.yml

✨ Highlights
--End-to-end automated static website deployment.
--HTTPS secured using free Cloudflare SSL.
--Fast, global delivery using Cloudflare CDN.
--Clean, minimal GitHub Actions setup.
