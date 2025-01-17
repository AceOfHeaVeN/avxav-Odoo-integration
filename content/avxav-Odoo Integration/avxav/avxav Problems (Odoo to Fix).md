---
title: '"avxav Problems (Odoo to Fix)"'
draft: true
tags:
---
up:: [[Odoo]] [[avxav]]

==The four major performance KPIs are:==

==1. Measure of Cost==

==2. Measure of Quality==

==3. Measure of Speed==

==4. Measure of Service==

---
## Finance

- Finance needed to prepare a check (Cheque) for iSystem, but the PO was not signed yet by the client because there was a delay from the logistics. They didn't send it in time for the client to sign before the checks were signed by the owner.
	- This meant that the check was not signed, and there was a week delay for getting the items from iSystem.
	- This meant we were 1 week late to the client.
	- We need to be able to create checks even if the PO wasn't signed due to human error, but the check itself cannot be delivered without the signed PO and the item can't be closed.
		- By Special approval from the manager.
		- The employee can raise the request to the manager clearly to be approved. Request can be approved with the press of a button.


- Do we need paper records? Can't we make it all digital?
	- I asked Mohannad, and he seems to be on board with an archiving solution for all invoices to be scanned and entered into the system efficiently.
	- It must be faster than the current procedures.
	- What's the cloud storage in Odoo.sh? Will it be able to hold all of these documents without issues?

---
## Inventory

- We deal with a large warehouses company called Naouri Group to store some of our orders.
	- When we want to get our inventory out. They request that we send them an email with very detailed information like serial number, etc.
	- And this information must be sent beforehand.
- Delays happen when the Logistics are overwhelmed and forget to send the inventory out request.
	- The system must help us in this regard by automating the process as much as possible.
		- For example, the logistics can choose that they want to send an email to Naouri, then quickly pick the items, their quantities, and when they want to pick them up. Then an automatic email is sent to Naouri with this info.

---
## Sales
- One of the problems that we face in most of our projects is making a profit in our projects, as we fail to estimate the actual cost of stuff due to improper planning prior to quoting the client. ^75389c
	- For example, clients often require Steel Structures to install the screens on, the sales guys do not know this cost, and they estimate it based on previous projects.
	- Other services like wench services, additional labor costs, storage costs, land or air freight costs, etc. are needed often.
	- A ==solution== to this might be to send a task to the department that is responsible for each cost:
		- Supply chain for the storage and freight costs.
		- Pre-sales for Steel structure, wench, and labor costs.
		- Then when all of these departments add their estimated costs, the sales team can then prepare the quotation.

- Another similar issue is with adding the correct Incoterms and payment terms: ^9f64ce
	- If the sales person is not very familiar with Incoterms, then they might add the wrong terms to the RFQ.
	- And sometimes, even if they add the correct payment terms as usually defined, the Finance department might have a different view depending on the current financial situation.
	- So adding approvals prior to sending the RFQ will be the ==solution== for this issue.

---
## Project Management

- We need to be able to track relationships between companies. For example, if we want to foster a relationship with a new company, we should be able to track the progress similar to an opportunity.
	- An example of this is the Steel Structures Company (Zain Project), we want to be on good terms with them, so that we can open up more business opportunities in the future.


- Creating project plans takes valuable time, what can we do to make those easier and faster to create?. Currently we do it in excel, but if there is a better recommendation, please let me know. ^3607c5



---
## Entire Company

### Finding the needed data without having to talk to another person:

- This is one of the major issues that we have in our company. When someone needs certain information like: ^899a53
	- Inventory quantity of a certain item.
		- And if this item is reserved for a certain client.
		- If this item has been installed as a mockup for a certain client.
	- The BOQ for a certain project.
		- I personally need this in order to complete CAD drawings by knowing the types and quantities of the screens.
	- The price for certain 3rd party services and items (Check this problem: [[avxav Problems (Odoo to Fix)#^75389c|Pricing Problem]])
- A ==Solution== Might be to create a standardized folder structure that the entire company can easily follow, making finding the required documents easy.
	- (Also check this: [[Questions to Ask Odoo#What is the best way to setup folder names (Folder Structures) for everyone in the company to be able to access the data that they need?|Question: Folder Structure]]).


---

See Also:
- [[Questions to Ask Odoo]]
- [[Ideas to Implement in Odoo]]