
|                   | Projects                                                                                            | Projects (classic)                                                                     |
| ----------------- | --------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Tables and boards | Boards, lists, timeline layout                                                                      | Boards                                                                                 |
| Data              | Sort, rank and group items by custom fields such as text, number, date, iteration and single select | Columns and cards                                                                      |
| Insights          | Create visuals to help understand your work through historical and current charts with Projects     | Progress bar                                                                           |
| Automation        | GraphQL API, Actions and Column                                                                     | Configure Column presets for when issues and pull requests are added, edited or closed |

***
### List of Project enhancements

**Tables and boards:**
- Track work in a table or board view
- Rank, sort and group within a table by any custom field
- Create draft issues with description and metadata
- Materialize any perspective with tokenized filtering and saved views
- Customize cards and group-by in Project boards
- Real-time updates and user presence indicators

**Data:**
- Custom fields of type: text, number, data, iteration and single select
- Configure iterations with flexible date ranges and breaks to represent your sprints, cycles or quarterly roadmap
- View linked pull requests and reviewers in table and board views

**Insight:**
- Create and configure custom bar, column, line and stacked area charts
- Use aggregation functions like sum, count, average, min and max to get proper insight
- Persist charts and share them with URL

**Automation:**
- GraphQL Projects V2 API
- GitHub app Project scopes
- Webhooks events for Project item metadata updates
- GitHub Action to automate adding issues

***
### Project access

**Organization-owned Project:**
- No access:
	- Only organization owners and users granted individual access can see the Project. Organization owners are also admins for the Project.
- Read:
	- Everyone in the organization can see the Project. Organization owners are also admins for the Project.
- Write:
	- Everyone in the organization can see and edit the Project. Organization owners are also admins for the Project.
- Admin:
	- Everyone in the organization is an admin for the Project.

**Personal/User-owned Project:**
- Read:
	- The individual can view the Project.
- Write:
	- The individual can view and edit the Project.
- Admin:
	- The individual can view, edit and add new collaborators to the Project.

