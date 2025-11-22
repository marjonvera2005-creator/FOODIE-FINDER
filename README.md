# Foodie Finder

A Django-powered web application to discover the best restaurants and dishes in Naval Proper.

## Features

✨ **User Experience**
- Preloader on page load with animated logo
- Personalized welcome messages
- Toast notifications for registration, login, errors
- Smooth scrolling effects

### Main Dashboard
- Smart search with autocomplete suggestions
- Category-based filtering system
- Featured restaurant cards with hover effects
- Menu preview with pricing information

### Restaurant Discovery
- Detailed restaurant profiles
- Image galleries and menus
- Opening hours and location info
- Category-based organization

### User System
- Secure authentication (login/register)
- Logout confirmation dialog
- User-friendly error handling
- Session management

### Responsive Design
- Mobile-first approach
- Tablet and desktop optimized
- Touch-friendly interactions
- Fast loading animations

## Technology Stack

- **Backend**: Django 4.2+ (Python)
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Database**: SQLite (dev) / PostgreSQL (production)
- **Styling**: Custom CSS with animations & gradients
- **Icons**: Font Awesome 6
- **Deployment**: Railway/Render ready

## Quick Start

### Prerequisites
- Python 3.11+
- Git

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/foodie-finder-naval.git
cd foodie-finder-naval
```

2. **Create virtual environment:**
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Setup database:**
```bash
python manage.py migrate
python manage.py createsuperuser
```

5. **Run development server:**
```bash
python manage.py runserver
```

6. **Visit:** `http://localhost:8000`
   - Restaurant users → Restaurant Dashboard for managing their restaurant
   - Regular users → Main Foodie Finder page
3. **Admin Features**: Manage restaurants, users, and system overview
4. **Restaurant Features**: Edit restaurant details, manage menu and images
5. **User Features**: Browse restaurants, search dishes, view details
6. **Role Management**: Admins can change user roles through Django admin panel

## Project Structure

```
├── core/               # Main application
│   ├── models.py      # Restaurant, Dish, Profile models
│   ├── views.py       # Views and logic
│   ├── admin.py       # Admin configuration
│   └── migrations/    # Database migrations
├── templates/         # HTML templates
├── static/            # CSS, images
│   ├── css/
│   └── img/
├── foodie_finder/     # Django settings
└── manage.py         # Django management script
```

## Technologies

- Django 5.2.7
- SQLite (default database)
- Pillow (image processing)
- HTML/CSS/JavaScript
- Poppins font (Google Fonts)

## Customization

### Adding Restaurants
Access the admin panel and use the Restaurant model to:
- Add new restaurants
- Upload images
- Set operating hours
- Assign categories
- Mark as featured

### Changing Theme Colors
Edit `static/css/styles.css` to adjust CSS variables:
```css
:root {
  --primary:#F54749;
  --accent:#FFB703;
  --green:#16a34a;
  --red:#dc2626;
}
```

## Notes

- All user data is stored in the database and visible only to admin
- The background image and logo are customizable in `static/img/`
- Restaurant images should be uploaded via admin panel
- Search suggestions cover A-Z popular dishes

## License

Created for educational purposes.

