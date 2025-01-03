# HL Project

Welcome to the **HL Project** repository! This is a Manual for the EMI testings.

## Features

- **Modular Design**: Separates different functionalities (e.g., `main`, `military`, `automotive`, `civilian`) using Flask Blueprints.
- **Blueprint Architecture:** Organized with a clear modular structure.
- **Customizable Structure**: Easily extendable for adding new sections or features.
- **Static Files Management**: Demonstrates handling of static files for multiple blueprints.
- **Dynamic Routing**: Includes examples of routing and URL generation using Flask's `url_for`.
- **NGINX Integration:** Configured for production-ready deployment.
- **Gunicorn Support:** Uses Gunicorn for WSGI server management.

---

## Project Structure

```plaintext
hl/
│
├── app/
│   ├── __init__.py                # Application factory for Flask
│   ├── main/                      # Main blueprint
│   │   ├── __init__.py            # Blueprint registration for main
│   │   ├── routes.py              # Routes for main
│   │   ├── static/                # Static files for main
│   │   │   ├── css/               # CSS files
│   │   │   ├── images/            # Images
│   │   ├── templates/             # Templates for main
│   │       ├── base.html          # Base template
│   │       ├── index.html         # Index template
│   ├── military/                  # Military blueprint
│   ├── automotive/                # Automotive blueprint
│   ├── civilian/                  # Civilian blueprint
│
├── venv/                         # Python virtual environment directory
├── .gitignore                    # Specifies files to ignore in version control
├── LICENSE                       # License information
├── README.md                     # Project documentation (this file)
├── app.py.delete.it              # Old entry point, marked for deletion
├── config.py                     # Application configuration settings
├── gunicorn.conf.py              # Gunicorn configuration file
├── requirements.txt              # Python dependencies
├── wsgi.py                       # Entry point for Gunicorn (runs the app)
