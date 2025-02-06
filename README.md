# Tweenter

A simple social media application built with Django.

## Features

- **User Authentication:** Secure registration, login, and password management.
- **Profile Management:** Customize profiles with biographies, profile pictures, and more.
- **Content Posting:** Create and manage posts in a Twitter-like interface.
- **Social Interactions:** Follow and unfollow other users to build a dynamic network.
- **Responsive Interface:** Modern and responsive UI implemented with Django templates.

## Project Structure

```
.idea/                          # IDE configurations


db.sqlite3

                      # SQLite database file


manage.py

                       # Django management script
templates/                      # Global templates folder
└── tweenterapp/                # App-specific templates (e.g., edit.html, login.html)
Tweenter/                       # Django project package (settings, urls, wsgi, etc.)
tweenterapp/                    # Main application (models, views, urls, tests, etc.)
twt_venv/                       # Virtual environment folder
```

## Setup and Installation

1. **Clone the Repository**

   ```sh
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Create and Activate a Virtual Environment**

   ```sh
   python -m venv twt_venv
   source twt_venv/Scripts/activate   # On Windows: twt_venv\Scripts\activate
   ```

3. **Install Dependencies**

   ```sh
   pip install -r requirements.txt
   ```

4. **Apply Database Migrations**

   ```sh
   python manage.py migrate
   ```

5. **Create a Superuser**

   ```sh
   python manage.py createsuperuser
   ```

6. **Run the Development Server**

   ```sh
   python manage.py runserver
   ```

   Open your browser and navigate to [http://127.0.0.1:8000/](http://127.0.0.1:8000/) to access the application.

## Technical Overview

Tweenter leverages Django’s robust architecture to deliver a feature-rich experience:

- **Models:** Custom models extend Django’s built-in `User` model for profile enhancements and post management. See 

models.py


- **Views & URLs:** Core functionality is implemented through views and URL configurations. Explore 

views.py

 and 

urls.py

 for more details.
- **Templates:** The user interface components and layouts are maintained within the templates/tweenterapp directory.

## Testing

Unit tests ensure the reliability of the application. Run tests using:

```sh
python manage.py test tweenterapp
```

## Contributing

Contributions are welcome. Please fork the repository, make your changes, and submit a pull request. For issues or feature requests, please use the repository's issue tracker.

## License

This project is licensed under the MIT License. See the LICENSE file for further details.
```
