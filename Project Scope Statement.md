# Project Scope Statement
## Overview
__Name:__ : Montani Style Distributed Order Management System (DOMS)

Client: Montani Style Industry: Retail & E-Commerce Project Manager: Sophia Shaw Budget: $750,000 – $1,000,000 (estimated) Date: 05 October 2026 Status: Waiting Approval

## Problem Statement
Montani Style is a national apparel retailer operating 45 brick-and-mortar stores alongside a growing e-commerce platform. 
Online and in-store inventory run on disconnected legacy systems. This causes frequent stockouts, expensive split shipments, 
and inflated return-processing costs. Store associates cannot fulfill online orders from local shelf stock because on-hand inventory data is unreliable in real time.

## Pain Points 
* Online and store inventory are separate, so stock is hard to see and often wrong
* Frequent stockouts online, even when stock is sitting in a store or warehouse
* High shipping costs because one order is often split into several packages
* Store managers cannot use local shelf stock to fill online orders
* Returns are slow and costly to process and are not reflected in inventory quickly

## Proposed Solution 
Develop a Distributed Order Management System (DOMS) that combines online and in-store inventory into a single source of truth. The system will:
* Keep one real-time record of stock for all stores, warehouses, and the website
* Route each online order to the best fulfillment location (warehouse or nearby store)
* Support "Buy Online, Pick Up In-Store" (BOPIS)
* Give store associates mobile tools for inventory audits and return processing
* Connect to the existing legacy systems instead of replacing them

## Project Goal
Create a system that sorts and tracks inventory automatically, 
reducing the errors that keep happening at Montani Style. Inventory management is one of the company's biggest challenges, 
so the project includes a mobile interface that helps store associates track stock more easily and reduces stockouts and system disconnects.

## In-Scope Deliverables

**Main deliverable:** a user-friendly interface (including a mobile version for store associates) to track and manage inventory across all 45 stores and the warehouses.

### Unified Inventory (`epic:inventory`)

- Real-time inventory record for every item at every location
- Automatic stock updates from store registers and warehouse systems
- "How many can we promise" calculation with a safety stock buffer
- Stock lookup and mobile stock counts (cycle counts)

### Order Routing (`epic:order-routing`)

- Online order intake
- Rules-based choice of the best store or warehouse
- Keeping orders in one package when possible
- Automatic rerouting when a location cannot fill an order
- Buy Online, Pick Up In-Store workflow (hold item, pick, notify customer, hand off)

### Location (`epic:location`)

- Store and warehouse location management
- Nearby-store stock lookup and preferred store
- Shipping addresses and package tracking
- Daily order limits for each store

### Store Associate Mobile Tools

- Mobile inventory audits
- Ship-from-store pick and pack
- In-store return processing, restocking, and refund trigger

### Integration, Security & Operations (`epic:integration`)

- Connectors to legacy register, warehouse, and website systems
- Role-based permissions and activity logs
- Monitoring, alerts, and nightly stock checks against legacy systems

### Reporting

- Dashboards for shipping cost, split shipments, inventory accuracy, and stockouts

### Support

- End-user documentation and staff training
- Pilot in 5 stores, then phased rollout to all 45 stores

---

## Out-Of-Scope Exclusions

- Replacing the legacy register, warehouse, or website systems
- Demand forecasting and automatic purchase orders
- Loyalty programs, promotions, and pricing tools
- A new customer mobile app (BOPIS uses the existing website)
- International expansion (other currencies, languages, customs)
- Buying hardware such as scanners or tablets
- RFID tracking

## Budget

**Estimated total: $750,000 – $1,000,000**

| Cost area | Estimate | Notes |
|---|---|---|
| Software development | About $250,000 | Writing the code and building the data needed for a smooth application |
| Rollout to all 45 stores | Remaining budget | Installation costs, staff training, and making sure employees can use the system |
| Testing and running the project during construction | About $200,000 | Needed for the best possible performance |

The rollout cost is not fixed yet. Once the development and testing estimates are subtracted, roughly $300,000 – $550,000 of the budget remains for rollout and training.

## Milestones

| Date | Milestone |
|---|---|
| 9/21 | Project Deliverable #1 |
| 10/2 | Project Deliverable #2 |
| 10/8 | Project Deliverable #3 |
| 10/19 | Project Deliverable #4 |
| 10/26 | Project Deliverable #5 |
| 11/9 | Project Deliverable #6 |
| 12/4 | Final Project Deliverable |

## Constraints

- $750,000 – $1,000,000 estimated budget
- Project deliverables are due between 9/21 and 12/4 (see Milestones)
- Stock lookups and searches must load within 3 seconds
- Stock changes must show across all channels within 60 seconds
- Legacy systems stay in place, so the new system must work with their limited connections
- The project must not expand PCI (payment card) scope, and customer data must follow privacy laws
- No rollout to stores during the November–December peak season
- Store staff can only spend about 1 hour each on training

## Assumptions

- Team members have the skills needed to meet project expectations
- Legacy register and warehouse systems can send stock changes (events, change logs, or polling every 5 minutes or less)
- Item and location data can be cleaned up before it is moved
- Stores have wifi and existing phones or tablets that can run the mobile tools
- Cloud and software prices will not increase greatly, and new regulations will not change the project while it is active
- Business stakeholders are available each sprint for reviews and testing
- The team will have all necessary resources to finish the project

---

## Team Roles

### Sophia Shaw – Project Manager, Scrum Master

- Define goals, schedules, roadmaps, and scope
- Manage day-to-day work, assign resources and tasks
- Monitor team coordination and execution, track performance
- Communicate with stakeholders
- Help the team work efficiently by removing roadblocks

### Noah Witzleb – Lead Business Analyst

- Gather and clarify project requirements from stakeholders
- Use data to find trends and measure results against the baseline
- Keep the backlog and user stories up to date
- Lead user testing and sign-off

### Kenley Elmore – Systems Architect

- Design the system architecture
- Ensure security and scalability
- Guide the technical work, including legacy system connections

## Stakeholders

- Montani Style management and project sponsor
- Store managers and store associates
- Online and in-store customers
- Warehouse and supply chain team
- E-commerce team
- Finance team
- IT, security, and legacy system owners
- Shipping carriers and payment providers
