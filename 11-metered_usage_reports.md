GitHub provides billing and consumption reports to track the usage of metered products. These reports helps monitor costs, allocate resources efficiently and ensure compliance.

***
### GitHub Actions minutes

***Free allocation:***
- Public repositories get unlimited free minutes.
- Private repositories receive free minutes based on the plan:
	- GitHub Free: 2000 minutes/month
	- GitHub Pro: 3000 minutes/month
	- GitHub Team: 5000 minutes/month
	- GitHub Enterprise: 50000 minutes/month
***Pricing per runner type:***
- Linux: $0.008 per minute
- Windows: $0.016 per minute
- macOS: $0.08 per minute

***Optimization strategies:***
- Use self-hosted runners for high-volume workflows to reduce costs
- Optimize workflow scripts by caching dependencies and reducing redundant jobs
- Limit workflows to only trigger when necessary

***
### Storage for GitHub Packages

**Free Allocation:**
- **Public repositories:** Free storage and bandwidth.
- **Private repositories:**
	- Storage up to 2GB
	- Data transfer up to 1GB per month

***Optimization strategies:***
- Regularly **delete unused packages** or enable retention policies.
- Store frequently accessed images in a **centralized registry** to reduce duplication.
- Use **compressed formats** to reduce storage consumption.

***
### GitHub Enterprise (GHE) Licenses

***Pricing Model:***
- Each user with access to private repositories consumes **one license**.
- Organizations pay per user annually or monthly.
***Inactive Users:***
- If an admin **removes** a user, the license remains **assigned** for the billing period but can be reallocated.

***Optimization strategies:***
- Audit **inactive users** and revoke access to free up licenses.
- Use **SSO and SCIM provisioning** to automate user management.

***
### GitHub Advanced Security (GHAS) Licenses

***Pricing Model:*** 
- Charged per unique committer per month. 
- If a committer contributes to multiple repositories, they only count once. 
***Free Tier:***
- Not available (only for public repositories).

***Optimization strategies:***
- **Restrict GHAS** to repositories that **truly need advanced security**.
- Use **branch protections** to limit unnecessary scans on feature branches.

***
### GitHub Copilot

***Access Model:***
- Available for individuals and businesses with different subscription options. 
***Free Access:***
- Free for students and verified open-source maintainers. 
- Free for select enterprise customers (trial-based).

***Optimization strategies:***
- Regularly **review and deactivate Copilot** for users who don’t need it.
- Encourage developers to **disable Copilot** in projects where AI-generated code is unnecessary.

***
### Large File Storage (LFS)

***Free Tier:***
- 1GB of storage per account per month
- 1GB of bandwidth usage per month

***Optimization strategies:***
- **Use external storage services** (e.g., AWS S3, Azure Blob Storage) for large files.
- **Delete unused large files** to optimize storage.
- **Enable Git LFS file pruning** to remove unreferenced objects.