### Method 1: Find license usage for a specific organization

Command-line (GraphQL APL):
``` JSON
{ 
	organization(login: "org-name") { 
		billingInfo { 
			totalSeats 
			seatsUsed 
			seatsAvailable 
		} 
	} 
}
```

***

### Method 2: Find license usage across multiple organizations

GraphQL API query for all organizations:
``` JSON
{ 
	enterprise(slug: "enterprise-name") { 
		organizations(first: 50) { 
			nodes { 
				name 
				billingInfo { 
					totalSeats 
					seatsUsed 
					seatsAvailable 
				} 
			} 
		} 
	} 
}
```

*** 

### Method 3: Find license usage for enterprise accounts

REST API:
``` Bash
curl -H "Authorization: token YOUR-TOKEN" \
"https://api.github.com/enterprises/YOUR-ENTERPRISE/license"
```

***

### Method 4: Find license usage across multiple GitHub instances

GitHub Enterprise Metrics API:
``` Bash
curl -H "Authorization: token YOUR-TOKEN" \
"https://api.github.com/enterprise/settings/licenses"
```

***

### Best practices for license usage management

***Automate monitoring*** - use GraphQL or REST API queries to track usage trends
***Reclaim unused seats*** - identify inactive users and free up unused licenses
***Enable usage-based billing*** - align billing with actual consumption
***Audit regularly*** - conduct monthly or quarterly reviews to control costs