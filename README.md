# Quotes Application

This is a simple Flask web application for managing and displaying favorite quotes. Users can view a list of quotes, add new quotes, and explore inspiring words.

## Features
- View a list of favorite quotes.
- Add new quotes via a user-friendly form.
- Quotes are stored in a PostgreSQL database.
- Responsive design for various devices.

## How to Use
1. *Clone the repository:*

    bash
    git clone https://github.com/yourusername/quotes-app.git
    

2. *Navigate to the project directory:*

    bash
    cd quotes-app
    

3. *Install dependencies:*

    bash
    pip install -r requirements.txt
    

4. *Configure the database:*
    - Set up a PostgreSQL database.
    - Update the database connection URI in app.py:

        python
        app.config['SQLALCHEMY_DATABASE_URI'] = 'your_database_uri_here'
        

5. *Set Flask environment variables:*
    - Create a .flaskenv file in the project root.
    - Add the following lines to set Flask environment variables:

        env
        FLASK_APP=app.py
        FLASK_ENV=development
        

    - Customize the FLASK_APP variable if your main Flask file is named differently.

6. *Run the Flask application:*

    bash
    flask run
    

7. *Open your web browser and navigate to [http://localhost:5000/](http://localhost:5000/) to view the list of quotes.*

8. *To add a new quote:*
    - Go to [http://localhost:5000/quotes](http://localhost:5000/quotes).
    - Use the "Add a quote" button.

## Project Structure
- *quotes.py:* Main Python file containing the Flask application.
- *templates:* Folder containing HTML templates for the application.
- *static:* Folder containing static assets such as CSS files.
- *requirements.txt:* file containing list of all the necessary pcakages


## Customize Database
To set up a different database or modify the connection details, update the SQLALCHEMY_DATABASE_URI variable in app.py.

```python
app.config['SQLALCHEMY_DATABASE_URI'] = 'your_database_uri_here'