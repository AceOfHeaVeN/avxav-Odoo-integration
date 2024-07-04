---
title: '"Business Cycle"'
draft: true
tags:
---
Ahmad = Sales / Sales Manager
Omar = Project Manager (PM)
Ola = Supply Chain Supervisor (SC)
Logistics and Procurement report to Ola.
Mohannad = Finance Manager

It begins with Sales

Lead gets in, Sales talks to them, 

We do site survey, then drawings or images. Once confirmed.

Then the BOQ is created by Ahmad, after asking me for drawings.

Then Sales sends to the supplier, to get a price from them,
- The price can be an official offer, or over the phone.

(قصة طرمة مع سلامة)
Problem with Sales:
Other personnel do not know about any sales until Ahmad decides to share it with them. How can we change this???
- If Ahmad gets a phone call from the client and forgets to input it in the system, how can we automate this?
- Can Odoo get call recordings or email communications and use AI to get this information?


Then Ahmad sends to Logistics to get the landed cost prices
- Then Logistics compares prices between multiple shipping suppliers
- Create a comparison sheet (Do negotiation plz)
- Take lowest price
- Create price fluctuation (from the screens supplier)
- Compare them with the costing that Ahmad made (This shouldn't even be a thing if the costing was made after approvals). (This happens because sometimes the logistics have a price for something ex: a mouse for 7USD, but then Ahmad sets the selling price for the mouse at 5USD and the cost at 3USD, so they have to then look up other prices that are lower than the 3USD cost to maintain the profit margin).
- Then they try to get lower prices.
	- Note: shipping prices can differ from the time the offer is sent to the client, and the time they pay us, however, the logistics try their best to match them.
	- This fluctuation percentage is usually included in the margin.
- You ask Ahmad for the price of?? (something Ola sent but didn't finish).


Also, sometimes Ahmad asks me or Omar for the price of the steel structure or glass for the project.
- Omar calls Art Media and asks them for a price.

Let's not forget Yazan's part in this, Ahmad sometimes asks him which Media Player, and PADS4 license.

Here we finished costing, then Ahmad adds his margin and sends the offer to the client.
- With Finance there are some other stuff that they do with the client (كفالة بنكية Bank Guarantee, Stamps, etc.).
- The Terms and Conditions are sent to the client.

After the client approves the offer and send us a PO with their own T&C, or sends an email confirmation, then Ahmad forwards this to email to Logistics and Finance.
- The BOQ is sent to the Project Manager and Yazan.

(Logistics convert the Price Offer from PDF to Excel to add their inputs and track the progress)
- The tracking should be always shown on the dashboard to all parties.
- Specially tracking of shipments, to able to answer clients about the arrival of shipments.

Logistics issue a PO for the supplier for all of the items inside of the BOQ except the items that are already in the inventory.

PO Approval Matrix:
- Based on supplier's quotation, and BOQ.
- Prepared by Logistics or Procurement.
- Approved by Supply Chain, Finance Manager.
	- Optional: PM, Sales Manager, Owner.
		- Per certain rule agreed upon in detail later.

PO is sent to the supplier, and the client signs and stamps it, then it is sent back to us.

Payment Terms:
- 

Omar needs to call the client to know when the Opening date for the branch is, what time we must have the screens delivered.

Waiting times (Customs clearance, shipping, testing of the screens).

Delivery Note Process:
- The PM sends SC that we need a delivery note for a certain project.

Goods Out Process:

Finance Invoice, Amend BOQ, Landed Cost then send to finance.

Handover then final invoice.

Sales and Cost, PSI, Inventory Report, etc.



Comments and Requests:
A problem for Logistics:
- Too many emails for tracking shipments, and for tasks.
	- Can we connect Odoo to automatically understand emails and then create tasks from them?
		- For example, if the logistics received three emails that contains a certain shipment with their departure and arrival dates.
- For POs, when reminding Finance to get payment from customers, or to pay the suppliers.
	- Can Odoo have automatic reminders set on certain dates?
	- Reminders for both Finance and for Logistics.


We are required to send POs to clients over 100JOD, this is an internal policy, this needs to be added to Odoo.


Testing products after they arrive, before sending it to the client.


When we create a client, we want to be able to set the payment terms (100% for example). Then the system creates automatic tasks or reminders for the Finance Department to pay then on the next Tuesday.
- This means that Odoo should be able to accommodate multiple times for reminders of the same task.
- For example we use natural language for dates, for example, in 7 days remind X about invoices, then 12 days after the invoices, remind Y that production is finished and you should start processing other stuff.


### 1. Sales Cycle:

- **Lead Generation:**
    - Lead gets in, Sales team (Sales Manager) talks to the lead.
- **Site Survey and Proposal:**
    - Conduct a site survey.
    - Create drawings or images.
    - Confirm with the client.
- **Bill of Quantities (BOQ):**
    - Sales Manager creates the BOQ after consulting for drawings.
- **Supplier Pricing:**
    - Sales sends the BOQ to the supplier for pricing (official offer or over the phone).
- **Internal Communication:**
    - Ensure all relevant personnel are informed about sales activities.
    - Explore automation for logging sales calls and email communications into Odoo using AI.

### 2. Logistics and Procurement:

- **Landed Cost Calculation:**
    - Sales Manager sends the BOQ to Logistics.
    - Logistics compares prices from multiple shipping suppliers.
    - Create a comparison sheet and negotiate for the lowest price.
    - Account for price fluctuations from the screen supplier.
    - Compare logistics prices with Sales Manager’s costing.
    - Obtain lower prices where possible.
- **Special Price Requests:**
    - Sales Manager or Project Manager requests prices for steel structures or glass.
    - Project Manager contacts Art Media for pricing.
    - Sales Manager consults Media Specialist for Media Player and PADS4 license.

### 3. Offer to Client:

- **Finalizing Costing:**
    - Sales Manager adds his margin to the costs.
    - Offer is sent to the client, including Terms and Conditions.
    - Finance handles bank guarantees, stamps, and other client-specific terms.
- **Client Approval:**
    - Client approves the offer and sends a PO or email confirmation.
    - Sales Manager forwards this confirmation to Logistics and Finance.
    - BOQ is sent to the Project Manager and Media Specialist.

### 4. Order Processing:

- **Order Tracking:**
    - Logistics converts the Price Offer from PDF to Excel for tracking.
    - Tracking progress is shown on the dashboard for all parties.
    - Special emphasis on shipment tracking for client inquiries.
- **Purchase Order (PO) Issuance:**
    - Logistics issues a PO for all BOQ items except those in inventory.
- **PO Approval Matrix:**
    - Based on supplier’s quotation and BOQ.
    - Prepared by Logistics or Procurement.
    - Approved by Supply Chain Supervisor and Finance Manager.
    - Optional approvals from Project Manager, Sales Manager, and Owner as per agreed rules.
- **Supplier Interaction:**
    - PO is sent to the supplier, signed, and stamped by the client, then returned to the company.

### 5. Project Execution:

- **Client Coordination:**
    - Project Manager contacts the client for the branch opening date and delivery timing.
- **Logistics and Customs:**
    - Manage waiting times for customs clearance, shipping, and screen testing.
- **Delivery Note Process:**
    - Project Manager requests a delivery note from Supply Chain for the project.

### 6. Delivery and Post-Delivery:

- **Goods Out Process:**
    - Execute the delivery of goods.
- **Finance Handling:**
    - Finance invoices, amend BOQ, calculate landed costs, and finalize the finance documentation.
- **Project Handover:**
    - Complete the project handover and issue the final invoice.
- **Reporting:**
    - Generate reports for sales, costs, PSI (Product and Service Inventory), and inventory.

### Key Issues Identified:

1. Lack of visibility on sales activities until Sales Manager shares information.
2. Manual logging of client interactions leading to potential oversights.
3. Price fluctuations and cost comparisons creating inconsistencies.

### Proposed Solutions:

1. Improve internal communication by automating logging of client interactions using Odoo’s capabilities.
2. Enhance visibility and tracking by displaying key metrics on a shared dashboard.
3. Standardize pricing and approval processes to minimize discrepancies and ensure consistency.