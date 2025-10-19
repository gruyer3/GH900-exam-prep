***Machine accounts*** and ***peripheral services*** (such as CI/CD, integrations and API consumers) can consume licenses.

***

***Machine accounts*** are accounts used for automation, running scripts or integrating with third-party tools.
***Characteristics:***
- They act independently of human users
- Often used by CI/CD tools
- Each machine account consumes a license, like a standard user

***

***Peripheral services*** are external integrations that interact with GitHub via API requests.
***Examples:***
- CI/CD pipelines
- Security scanning tools
- Third-party integrations
- Self-hosted GitHub Runners

***

### Finding Usage Statistics for Machine Accounts

#### Method 1: GitHub Enterprise Admin Console
1. Navigate to Enterprise Settings.
2. Select Billing & License Management.
3. Look for a Machine Accounts section.
4. Identify:
	- Number of active machine accounts.
	- License consumption per machine account.
	- Last active date.

#### Method 2: GraphQL API Query for Machine Accounts

``` JSON
{ 
	enterprise(slug: "enterprise-name") { 
		organizations(first: 50) { 
			nodes { 
				name 
				machineAccounts { 
					totalCount 
					nodes { 
						login 
						createdAt 
						lastActiveAt 
					} 
				} 
			} 
		} 
	} 
}
```

***

### Finding License Usage for Peripheral Services

#### Method 1: GitHub Actions & Runners Usage Metrics
1. Go to Enterprise Settings -> Actions
2. View:
	- Total GitHub-hosted runner minutes used.
	- Self-hosted runner usage.
	- Billing for extra runner minutes.

#### Method 2: REST API for Self-Hosted Runners
``` Bash
curl -H "Authorization: token YOUR-TOKEN" \ "https://api.github.com/enterprises/YOUR-ENTERPRISE/actions/runners"
```
Key insights:
- Identifies how many runners are consuming licenses.
- Track idle runners that may be wasting resources.
- Helps optimize billing for GitHub-hosted runner minutes.

#### Method 3: Peripheral Services API Usage Tracking
``` Bash
curl -H "Authorization: token YOUR-TOKEN" \ "https://api.github.com/enterprises/YOUR-ENTERPRISE/audit-log"
```
This helps you:
- Detect inactive services: find services no longer in use.
- Audit third-party tools: ensure external tools are necessary and properly configured.
- Reduce costs: disable services that are not providing value.

***

### Best practices for managing machine accounts & peripheral services licenses

1. Audit machine accounts regularly
2. Monitor API usage
3. Optimize runner usage
4. Restrict machine accounts