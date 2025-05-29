         
# Mirpur Dental Supply

A web application for managing dental supplies and inventory for Mirpur Dental Supply store. Built with Django, Tailwind CSS, and Alpine.js.

## Features

- Modern, responsive UI using Tailwind CSS
- Interactive components with Alpine.js
- Django backend for robust data management
- User authentication and authorization
- Product catalog and inventory management
- Order processing and tracking
- Reporting and analytics

## Tech Stack

- **Backend**: Django
- **Frontend**: 
  - Tailwind CSS for styling
  - Alpine.js for interactivity
- **Database**: SQLite (development), PostgreSQL (production recommended)

## Prerequisites

- Python 3.12+
- pip
- virtualenv (recommended)

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/mirpurdentalsupply.git
   cd mirpurdentalsupply
   ```

2. Create and activate a virtual environment
   ```bash
   python -m venv venv
   .\venv\Scripts\activate  # On Windows
   # source venv/bin/activate  # On macOS/Linux
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Create a local settings file
   ```bash
   copy examples\local_settings.example mirpurdentalsupply\local_settings.py
   # Edit the file with your specific settings
   ```

5. Run migrations
   ```bash
   python manage.py migrate
   ```

6. Create a superuser
   ```bash
   python manage.py createsuperuser
   ```

7. Run the development server
   ```bash
   python manage.py runserver
   ```

8. Visit http://127.0.0.1:8000/ in your browser

## Project Structure

```
├── Homepage/               # Main app for the website
│   ├── templates/          # HTML templates
│   │   ├── Homepage/       # App-specific templates
│   │   └── base.html       # Base template for the site
│   ├── views.py            # View functions
│   ├── urls.py             # URL routing
│   └── models.py           # Data models
├── mirpurdentalsupply/     # Project settings
│   ├── settings.py         # Main settings
│   ├── local_settings.py   # Local environment settings
│   └── urls.py             # Main URL routing
├── staticfiles/            # Collected static files
├── examples/               # Example configuration files
└── requirements.txt        # Python dependencies
```

## Development

### Adding New Apps

```bash
python manage.py startapp appname
```

Remember to add the new app to `INSTALLED_APPS` in `settings.py`.

### Collecting Static Files

```bash
python manage.py collectstatic
```

### Running Tests

```bash
python manage.py test
```

## Deployment

Example deployment configurations are provided in the `examples/` directory:

- `nginx.example`: Nginx configuration
- `uwsgi.example`: uWSGI configuration
- `service.example`: Systemd service file

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

Your Name - 2020tanvir1971@gmail.com

Project Link: [https://github.com/Tanvir-yzu/mirpurdentalsupply](https://github.com/Tanvir-yzu/mirpurdentalsupply)

        