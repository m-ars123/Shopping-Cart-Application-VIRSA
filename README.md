====================================================================
                    SHOPPING CART APPLICATION
                    =========================
====================================================================

A Flask-based Shopping Cart Web Application with SQLite database

====================================================================
                          QUICK START
====================================================================

Follow these steps to set up and run the project on your computer:

1. INSTALL PYTHON (If not already installed)
   ------------------------------------------
   • Download Python 3.7 or higher from: https://www.python.org/downloads/
   • During installation, CHECK "Add Python to PATH"
   • Verify installation: Open terminal and type: python --version

2. DOWNLOAD AND EXTRACT THE PROJECT
   ---------------------------------
   • Extract the ZIP file to a folder of your choice
   • Example: C:\Users\YourName\Desktop\shopping-cart-app\

3. OPEN PROJECT DIRECTORY
   -----------------------
   • Open Command Prompt, PowerShell, or Terminal
   • Navigate to the project folder:
     cd "C:\Users\YourName\Desktop\shopping-cart-app\"

4. SETUP VIRTUAL ENVIRONMENT (Recommended)
   ---------------------------------------
   • Create virtual environment:
     python -m venv venv
   
   • Activate virtual environment:
     - Windows: venv\Scripts\activate
     - Mac/Linux: source venv/bin/activate
   
   • You'll see (venv) in your terminal when activated

5. INSTALL REQUIRED LIBRARIES
   ---------------------------
   • Make sure virtual environment is activated
   • Install dependencies:
     pip install -r requirements.txt

6. RUN THE APPLICATION
   --------------------
   • Start the Flask server:
     python app.py
   
   • You should see output like:
     * Running on http://127.0.0.1:5000
     * Running on http://localhost:5000

7. ACCESS THE APPLICATION
   -----------------------
   • Open your web browser
   • Go to: http://localhost:5000
   • You should see the login page

====================================================================
                      TEST ACCOUNTS
====================================================================

Two pre-configured accounts are available:

ADMIN ACCOUNT:
-------------
Username: arsalan@gmail.com
Password: 123

CUSTOMER ACCOUNT:
----------------
Username: arsal@gmail.com
Password: 123

====================================================================
                    TROUBLESHOOTING
====================================================================

COMMON ISSUES AND SOLUTIONS:

1. "No module named 'Flask'"
   • Make sure virtual environment is activated (see (venv) in terminal)
   • Run: pip install Flask

2. Port 5000 already in use
   • Change port in app.py (last line):
     app.run(debug=True, port=5001)
   • Then access: http://localhost:5001

3. Database connection errors
   • Make sure CEP.sqlite file is in the project folder
   • If missing, the app will create it automatically

4. Virtual environment not activating (Windows)
   • Run this command first: Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
   • Then try: venv\Scripts\activate

====================================================================
                    PROJECT STRUCTURE
====================================================================

shopping-cart-app/
├── app.py                 # Main application file
├── CEP.sqlite            # SQLite database (auto-created)
├── requirements.txt      # Python dependencies
├── Procfile             # For deployment (ignore locally)
├── templates/           # HTML template files
│   ├── login.html
│   ├── signup.html
│   ├── products.html
│   ├── cart.html
│   └── ... (other HTML files)
├── static/              # Static files (CSS, images)
│   └── (product images)
└── product_images/      # Uploaded product images

====================================================================
                    DATABASE MANAGEMENT
====================================================================

VIEWING THE DATABASE:
---------------------
• Install DB Browser for SQLite: https://sqlitebrowser.org/dl/
• Open CEP.sqlite with DB Browser
• Browse tables: Users, Products, Cart, Orders, etc.

DATABASE TABLES:
---------------
1. Users          - User accounts (admin/customer)
2. Products       - Product catalog with images
3. Cart           - Shopping cart items
4. Orders         - Order history
5. OrderDetails   - Order line items
6. Feedback       - Product reviews and ratings

====================================================================
                    KEY FEATURES
====================================================================

• User authentication (Login/Signup)
• Product browsing and management
• Shopping cart with quantity management
• Order history tracking
• Admin panel for product management
• Responsive web design
• SQLite database for data persistence

====================================================================
                    USAGE GUIDE
====================================================================

FOR CUSTOMERS:
1. Login with customer account
2. Browse products on Products page
3. Add products to cart with desired quantities
4. View/update cart on Cart page
5. Checkout to place order
6. View order history on Shopping History page

FOR ADMINS:
1. Login with admin account
2. Access Admin Panel from navigation
3. Add new products (name, price, stock, image)
4. Update existing products
5. Remove products
6. View all orders in Order Manager

====================================================================
                    TECHNICAL DETAILS
====================================================================

TECHNOLOGIES USED:
-----------------
• Backend: Python, Flask, SQLite
• Frontend: HTML, CSS, Bootstrap, JavaScript
• Database: SQLite3

PYTHON DEPENDENCIES:
-------------------
• Flask==3.1.1
• itsdangerous==2.2.0

SYSTEM REQUIREMENTS:
-------------------
• Python 3.7 or higher
• 100MB free disk space
• Web browser (Chrome, Firefox, Edge, etc.)
• Internet connection (for Bootstrap CDN)

====================================================================
                    DEVELOPMENT
====================================================================

RUNNING IN DEBUG MODE:
----------------------
• The app runs in debug mode by default
• Auto-reloads when code changes
• Detailed error pages

CUSTOMIZING:
-----------
• Change port: Modify app.run(port=XXXX) in app.py
• Change secret key: Modify app.secret_key in app.py
• Change database: Modify DataHandler.DB_FILE in app.py

====================================================================
                    SUPPORT
====================================================================

If you encounter issues:
1. Check the Troubleshooting section above
2. Verify all installation steps were followed
3. Check terminal for error messages
4. Ensure CEP.sqlite file exists in project folder
5. Make sure all template files are in templates/ folder

For additional help, contact the project maintainer.

====================================================================
                    LICENSE
====================================================================

This project is for educational purposes.
Created as a Web Technology Project.

====================================================================
