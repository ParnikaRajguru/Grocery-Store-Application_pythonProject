This project is a simple Grocery Management System with modules for Products and Orders.
 Products Module

Edit Product

Earlier, we could only delete products.

Now, we added an Edit button next to the Delete button.

This lets us update product details (like name, price, UOM) without removing them.

Add New UOM (Unit of Measure)

Before, UOMs were fixed (Kg, Liter, Pack).

We added a form to create new UOMs (for example: Cubic Meter for wood).

This required:

Backend: Python server updated to store UOMs.

Frontend: UOM dropdown now loads dynamically with all available UOMs.

Orders Module

Form Validation

Before, orders could be placed with missing info.

Now, we added checks:

Customer name cannot be empty.

Item name must be valid.

Quantity must be greater than 0.

Grand Total Bug Fixed

Problem: If someone changed the total price of an item, the grand total did not update.

Fix: Grand total now recalculates whenever item totals are edited.

View Order Details

Added a View button in the orders list.

Clicking it shows complete order details:

Items inside the order

Quantity and price of each item

Total cost

How to Run

Start backend server:

python server.py


Open frontend app in browser.

Explore the changes:

Products → Edit / Add UOM

Orders → Validations / View Order / Fixed Totals
