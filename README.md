# Django and React App!

Union of Django for backend and React for frontend, the application shows a list of customers where the basic CRUD operations can be done. (Becoming an Ecommerce).

Separated into 3 main folders
 - DjangoProject (Django project configuration).
- Customers (Customers App - Backend).
- Frontend (React that consumes endpoints from the Customers App).

## Setup App

 1. Clone this repository: `git clone https://github.com/FabianAlvaradoDonoso/Django-React-Project.git`
 2. Create a virtual environment:  `python3 -m venv ./env`
 3.  Activate it  ☝️:  `source venv/bin/activate`  or  `venv\Scripts\activate`  if you're on a Windows.

### Backend Setup

 1. Install dependencies:  `pip3 install -r requirements.txt`
 2. Migrate the database: 
	```
	python manage.py makemigrations
	python manage.py migrate
	```
 3. To run the program in local server use the following command: `python manage.py runserver`

Server will be available at `http://127.0.0.1:8000` in your browser.


### Run (Frontend)

 1. Navigate the current working directory to `frontend`: `cd frontend`.
 2. Install the all frontend dependencies using npm:  `npm install`.
 3. Run the server:  `npm start`.

Frontend app will be available at `http://127.0.0.1:3000` in your browser.

## Endpoints

 - `/api/customers`: This endpoint is used to create customers and returns paginated sets of customers.
 - `/api/clusters/<pk>`: This endpoint is used to get, update, and delete individual clients by primary key or id.
