---
title: First Accounting Meeting 25-Jun-2024
draft: true
tags:
---
MOMs:

Today's meeting with Hamilton's Diala (Project Manager) and Abdallah Al Lala (CFO) was very interesting and fast-paced.

The meeting basically went as follows:
- The CFO Started by asking us questions related to the processes that the Accounting and Finance do on a daily bases.
	- This quickly escalated into very deep examples of those processes, and how Odoo could help us implement these complex processes.
	- Many of the features that we discussed needed customization, and were not supported by the Standard Odoo app.
- Phase 1 of the project included information gathering for Finance, Accounting, Supply Chain, and Sales.
	- In this meeting we discussed the first three, and sales will be done at a later time.
- The First topic that we discussed in this meeting was the warehouses and inventory tracking.
	- We discussed having physical warehouses and many virtual warehouses.
		- Transit, Hot Swap, Mockup, etc.
	- We discussed having 3rd party warehouse services via Naouri.
	- We gave them heaps of examples of how the process usually goes, and details of the complexity of it.
		- Ex: We purchase items for a project that is very long term, during this time, we might use the inventory to install the screens for another project, and then refill the used quantities later on.
			- We discussed how this impacts the GL and how to manage the differences in inventory (and possibly different screen models) using Odoo.
	- We discussed that the **Shelf Management** feature in Odoo is essential for us.
	- We would like to know if Odoo supports "*Read Receipts*" in Emails.
- Then we moved on to costing and how we process transactions.
- We also discussed the approval process and what that looks like.
	- Ex: If the Sales team wanted to do provide a quote to a client that requested different aspects like:
		- Software Licenses and Media Players.
			- Must be approved by the **Managed Services Department**.
		- Shipping and Landed Costs.
			- Must be approved by the **Supply Chain and Logistics Department**.
		- 3rd Party Construction works (ex: Steel Structure, Glass, Extra Workers, Cranes, etc.).
			- Must be approved by the **Project Management Department**.
		- In other special and urgent cases, the entire approvals process can be overridden completely. ^Approvals-Override-Question
			- This is usually a request by the owner to the sales team to send an offer immediately.
			- How shall we handle this?
	- That was just an example, but the approval workflows will be used in almost all tasks that require cooperating with other departments.
- We briefly discussed transferring HR from Minaitech to Odoo, but we need to study it for two reasons:
	- The HR needs to study if Odoo supports all the features that Menaitech supports.
	- That we have the needed amount of users for this transfer (Highly unlikely).
- We discussed that we needed **Budgeting** and **Cost & Profit Centers** Apps.
- We also require the **Repair & Maintenance** App.
- We discussed that we do not require the **Quality Checks** App, since approvals in workflows is more than enough.
- We require the **Documents** and the **Sign** Apps.
	- **Documents** App works like One Drive for the entire company, and access rights determines who can see which files.
	- **Documents** also has built-in apps that are similar to Word, Excel, etc.
	- The **Sign** App allows us to sign documents digitally, add our initials to every page, and stamp every page as needed.
- Finally, Odoo allows us to do everything from inside of it, without needing to switch apps:
	- For example, we can send emails directly from Odoo, this includes full conversations (Replies and CCs) and attachment management.
	- However, this doesn't mean that we will never use Excel for example, but having automations in the system will greatly reduce friction in our processes.
