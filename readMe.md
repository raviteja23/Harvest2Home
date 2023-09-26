Harvest home coming
Harvest home coming is a web application built using the Flask web framework that allows farmers to list their products for sale and customers to browse and purchase those products online.

Installation

Navigate to the project directory and create a virtual environment: python -m venv venv.
Activate the virtual environment: source venv/bin/activate (on macOS/Linux) or venv\Scripts\activate (on Windows).
Install the required dependencies: pip install -r requirements.txt.
Create a .flaskenv file in the project directory with your configuration variables, such as the database URI, secret key. 
An example .flaskenv file is provided in the project directory.

Database
The project uses a SQL database to store data. To access the database in the Flask shell, run the following commands:

$ flask shell
>>> from app import app
>>> from app import db
>>> db.create_all()

Set the FLASK_APP environment variable: export FLASK_APP=app.py
Initialize the database: flask db init
Create the initial migration: flask db migrate -m 'Initial migration'
Apply the migration to the database: flask db upgrade
Run the application: flask run.

Once the server is running, open a web browser and go to http://localhost:5000. You should see the home page.

Usage
Registering as a Farmer
Navigate to the registration page and select "Farmer" as your account type.
Fill in the registration form with your personal details and create a password.
Once registered, log in to your account and create a profile by adding your farm name, description, and location.
Add your products to your profile by providing their name, description, category, and price.
Browsing Products
Navigate to the "Browse Products" page to see a list of available products.
Filter products by category or search for specific products by name.
Click on a product to see more details and add it to your cart.
Checking Out
Navigate to your cart to review your order and make any adjustments.
Fill in your shipping and payment details and submit your order.

Registering as a user
Navigate to update details like username, location
User should be able to view products, select products, quantity, add to cart, get total price and check out
generate invoice.

