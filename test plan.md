🧾 TEST PLAN DOCUMENT

Project Title: Online Bookstore System
Version: 1.0
Prepared by: TNNP Team
Date: 3 November 2025

1️⃣ Introduction

The Online Bookstore is an e-commerce web application allowing customers to browse, search, and purchase books.
It also provides administrative capabilities for inventory and order management.
This Test Plan defines the strategy, scope, objectives, resources, schedule, and deliverables required to verify and validate the system.

2️⃣ Objectives

Ensure all core functionalities (catalog, user accounts, cart, checkout, inventory, order tracking) meet functional and non-functional requirements.

Verify data accuracy and transaction integrity.

Detect and resolve defects before release.

Confirm usability, performance, and security under expected workloads.

3️⃣ Scope
In-Scope
Category	Areas Covered
Functional	Book catalog, search, user registration/login, shopping cart, checkout, order tracking, inventory updates
Non-Functional	Usability, performance (page load ≤ 3 s), security (password encryption, session timeout), compatibility (Chrome, Edge, Firefox)
Data	MySQL database validation (user data, book info, transactions)
Out-of-Scope

Mobile app testing (future release)

Third-party payment gateway internal validation

Localization or multi-language support

4️⃣ Test Items
Module	Description
Book Catalog	Browse and search books by title, author, genre, ISBN
Authentication	Register, login, logout, password reset
Shopping Cart	Add, update, remove items
Checkout	Billing, shipping, and payment process
Inventory	Admin stock updates and synchronization
Order Tracking	Customer order status and history
5️⃣ Test Strategy
Test Type	Approach
Functional Testing	Black-box testing with requirement-based test cases
Integration Testing	Validate interaction between catalog, cart, and payment modules
System Testing	End-to-end workflow from login → checkout → order tracking
Regression Testing	Run automated tests after each build
Performance Testing	Measure response times and scalability under load
Usability Testing	Assess layout, readability, and navigation ease
Security Testing	Verify authentication, data privacy, and SQL injection resilience
6️⃣ Test Environment
Component	Details
OS	Windows 10 / 11, Ubuntu 22.04
Browser	Chrome v130+, Firefox v125+, Edge v130+
Backend	Node.js / Express, REST API
Database	MySQL 8.x
Tools	Postman, Selenium, Jest, GitHub Issues, Chrome DevTools
Test Data	Sample users, mock book catalog (≥ 50 books), test payment data
7️⃣ Test Deliverables

Test Plan Document (this file)

Test Case Document (Bookstore_TestCases.xlsx)

Defect Report (Bookstore_BugReport.xlsx or GitHub Issues)

Test Summary Report (final stage)

Test Execution Logs and Screenshots

8️⃣ Entry & Exit Criteria
Entry Criteria	Exit Criteria
✅ All functional modules developed and unit tested	✅ 100 % test cases executed
✅ Test environment configured and accessible	✅ 95 % test cases passed
✅ Valid test data prepared	✅ Critical and high-severity defects closed
9️⃣ Schedule
Phase	Start Date	End Date	Responsibility
Test Planning	Oct 28 2025	Oct 30 2025	QA Lead
Test Case Design	Oct 30 2025	Nov 2 2025	QA Team
Test Execution	Nov 3 2025	Nov 8 2025	Testers
Defect Reporting & Retesting	Nov 9 2025	Nov 12 2025	QA Team
Final Report	Nov 13 2025	Nov 14 2025	QA Lead
🔟 Risk Analysis
Risk ID	Description	Impact	Probability	Mitigation
R1	Payment API failure	High	Medium	Mock API for testing, retries
R2	Server downtime	High	Low	Deploy on local + backup
R3	Data corruption in checkout	Critical	Low	Database backups, rollback tests
R4	Poor performance under heavy load	High	Medium	Conduct load testing before release
R5	Session timeout not handled	Medium	Medium	Simulate idle scenarios
R6	Cross-browser rendering differences	Medium	High	Test on multiple browsers
1️⃣1️⃣ Metrics
Metric	Formula	Target
Test Case Execution Rate	Executed / Planned × 100	≥ 95 %
Defect Density	Defects / KLOC	≤ 0.5
Defect Removal Efficiency	(Resolved / Total Found) × 100	≥ 90 %
Test Pass Rate	Passed / Executed × 100	≥ 90 %
1️⃣2️⃣ Roles & Responsibilities
Role	Name	Responsibilities
QA Lead / Test Manager	Oversees plan, schedule, and progress	
Test Engineer	Designs & executes test cases	
Automation Engineer	Develops automated regression scripts	
Developer (Support)	Fixes reported defects	
Product Owner	Approves final release	
1️⃣3️⃣ Test Tools

Manual Testing: Postman, Chrome DevTools

Automation: Selenium WebDriver, Jest

Defect Tracking: GitHub Issues

Version Control: Git / GitHub

Reporting: Excel / Allure Reports

1️⃣4️⃣ Approval & Sign-Off
Name|	Role	|Signature|	Date|
DoMinic kirui|Test manager | DK|3rd nov 2025|		
|||||
||||||			
		
✅ Summary

This Test Plan ensures all functional and non-functional aspects of the Bookstore are validated before release.
The structured approach prioritizes risk-based testing, clear defect tracking, and measurable quality metrics.
