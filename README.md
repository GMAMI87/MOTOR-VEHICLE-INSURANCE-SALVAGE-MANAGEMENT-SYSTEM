# Motor-Vehicle-Insurance-Salvage-Management-System
Motor Vehicle Insurance Salvage Management System database
# ABSTRACT
The Motor Vehicle Insurance Salvage Management System is a web‑based internal tool that digitizes the buying and selling of insurance salvage vehicles. It replaces notebooks and spreadsheets with a structured, database‑driven solution that allows users to record salvage purchases, capture previous owner and logbook details, manage buyers, track sales, update vehicle status, and calculate profit automatically.
The system is built using Python, Streamlit, SQLite, Pandas, CSV handling, and Object‑Oriented Programming to enhance data accuracy, financial tracking, reporting efficiency, secure access control, and overall business scalability.

# INTRODUCTION
Most salvage businesses manage records using notebooks or Excel, creating inefficiencies such as difficulty tracking profit, poor linkage between buyers and vehicles, slow data retrieval, and lack of controlled access. As business volume increases, these limitations make operations error‑prone and hard to manage.
This project introduces a centralized, searchable, and secure management system built with Streamlit and SQLite. It improves accuracy, reporting, authentication, data validation, and usability through structured digital workflows.

# PROBLEM STATEMENT
Manual processes lead to:
• Lost, inconsistent, or duplicated records
• Inaccurate profit tracking
• Poor linkage between vehicles, buyers, and sales
• No secure authentication or restricted permissions
• Limited reporting visibility
• Reduced scalability
A secure, automated system is necessary to streamline operations, improve decision‑making, and enhance financial transparency.

# OBJECTIVES
# Main Objective
To design and implement a secure, database-driven salvage vehicle management system that digitally records and tracks all vehicle, buyer, and sales transactions.
# Specific Objectives
• Record salvage vehicles purchased from insurance companies
• Capture previous owner and logbook details
• Manage buyer information
• Link sales to specific vehicles and buyers
• Automatically update vehicle status
• Calculate and display profit
• Provide advanced search and filtering
• Generate dashboard analytics
• Export records to CSV for reporting
• Validate user inputs and provide user-friendly error messages
• Secure admin-only functions through authentication
• Apply OOP for modularity and future scalability
# SCOPE OF THE SYSTEM
The system includes:
• Vehicle management
• Buyer management
• Sales recording
• Automatic profit calculation
• Search and filtering (by reg number, status, insurance company, buyer)
• Dashboard reporting and summary metrics
• CSV export for Excel reports
• Admin login and restricted actions
It is designed for internal business use.
# TECHNOLOGY USED
• Python – core business logic
• Streamlit – interactive web UI
• SQLite – relational database
• Pandas – analytics and reporting
• CSV – export functionality
• OOP principles – maintainability and scalability

# SYSTEM DESIGN
1. Database Design
The system uses three relational tables:
# Motor Vehicles Table
vehicle_id, insurance_company, previous_owner, contact, logbook_number, registration_number, make, model, year, damage_type, purchase_price, selling_price, status
# Buyers Table
buyer_id, full_name, phone_number, id_number
# Sales Table
sale_id, vehicle_id (FK), buyer_id (FK), sale_price, sale_date
# 2. System Architecture
Streamlit UI → Python Application Logic (OOP) → SQLite DB Layer → Pandas Analytics → CSV Export

# KEY SYSTEM FEATURES
1. Search and Filtering
Search by registration number, filter by availability status, insurance company, or buyer. This speeds up data retrieval and improves traceability.
2. Dashboard & Reporting
The dashboard displays:
• Total vehicles purchased
• Vehicles sold
• Total purchase value
• Total sales revenue
• Total profit
• Profit per vehicle (bar chart)
3. Data Export
Users can export records to CSV for Excel-compatible reporting.
4. Security and Access Control
• Admin login authentication
• Session-based control
• Restricted edit/delete/export actions
5. OOP Code Structure
Classes include Vehicle, Buyer, Sale, Database, Authentication — improving reusability, logic separation, and future expansion.
6. Error Handling & Validation
The system validates:
• Required fields
• Positive numeric values
• Duplicate registration numbers
• Incorrect login attempts
• Empty/invalid input
Clear feedback messages are shown to guide the user.
FILE STRUCTURE
motor‑vehicle‑salvage-system/
• app.py
• database.py
• models.py
• auth.py
• salvage.db
• requirements.txt
TESTING
Testing verifies that:
• Vehicles and buyers are added correctly
• Sales link correctly to vehicles and buyers
• Status updates automatically after sale
• Profit calculations are accurate
• Search/filters work
• Dashboard totals are correct
• CSV exports are accurate
• Unauthorized access is blocked
DEPLOYMENT
Deployment through Streamlit Cloud:
Upload to GitHub → Create Streamlit App → Select app.py → Deploy → Share link.
SUCCESS CRITERIA
The system is successful if it:
• Stores accurate data
• Correctly links buyers and vehicles
• Updates status automatically
• Calculates profit accurately
• Produces accurate dashboard metrics
• Provides correct search/filter results
• Enforces secure login
• Generates proper CSV exports
FUTURE ENHANCEMENTS
• PDF and Excel export
• Role-based access (Admin vs Staff)
• Cloud database integration
• Automated profit summaries
• Mobile-friendly interface
• Backup and restore options
CONCLUSION
The system delivers a secure, scalable, and structured way to manage insurance salvage operations. Through Python, Streamlit, SQLite, Pandas, and OOP principles, it enhances accuracy, reporting, security, and business efficiency—making it suitable for real operational environments.
