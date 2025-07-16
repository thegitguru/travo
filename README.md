# Travo - Spiritual Travel Platform

!<img src="logo.jpeg" width="300" alt="Travo Logo">

**Repository**: [https://github.com/thegitguru/travo.git](https://github.com/thegitguru/travo.git)  
**Author**: [@thegitguru](https://github.com/thegitguru)

## Overview

Travo is a web application designed to offer spiritual travel packages to sacred destinations in India, such as Varanasi and Ayodhya. The platform provides a user-friendly interface for browsing travel packages, booking trips, and managing user accounts, with a robust admin panel for managing users and bookings. Built with modern web technologies, Travo emphasizes responsive design, accessibility, and a seamless user experience.

## Features

- **User-Facing Features**:
  - Browse spiritual travel packages to sacred destinations in India.
  - Secure user registration and login system.
  - Booking system for reserving travel packages.
  - Newsletter subscription for updates on new destinations and offers.
  - Responsive design for seamless use on desktop, tablet, and mobile devices.

- **Admin Panel Features** (Accessible at `/admin.html`):
  - **Dashboard**: Displays key metrics (total users, total bookings, active bookings) with a Chart.js bar chart for user growth trends.
  - **User Management**: View, edit, and delete user accounts with a responsive table and search functionality.
  - **Booking Management**: View and cancel bookings with a responsive table and search by email or destination.
  - **Modals**: Interactive modals for viewing/editing user details and viewing booking details, with input validation.
  - **Custom Buttons**: Distinct colors for actions (View: blue, Edit: orange, Cancel: red, Delete: dark red) with hover and focus states.
  - **Responsive Tables**: Horizontal scrolling on mobile, with stacked layout and data labels on very small screens (<576px).
  - **Sidebar Navigation**: Collapsible sidebar with smooth animations for navigating between dashboard, users, and bookings sections.
  - **Accessibility**: ARIA attributes, focus trapping, and keyboard navigation for modals and sidebar.

- **Design**:
  - Consistent aesthetic using the Saira font and a color palette with `--primary-color: #e63939` and `--secondary-color: #f06595`.
  - Animations (e.g., `fadeInUp` for cards, `slideIn` for sidebar) for a modern feel.
  - Fully responsive layout with breakpoints for desktop (>992px), tablet (768px–992px), mobile (<768px), and very small screens (<576px).

## Technologies Used

- **Frontend**:
  - HTML5, CSS3, JavaScript
  - Bootstrap 5 for responsive layout and components
  - Chart.js for dynamic data visualization
  - Font Awesome for icons
  - Saira font (Google Fonts) for typography
- **Development Tools**:
  - Git for version control
  - GitHub for repository hosting
- **Dependencies**:
  - Bootstrap 5 (`cdn.jsdelivr.net/npm/bootstrap@5.3.0`)
  - Chart.js (`cdn.jsdelivr.net/npm/chart.js@4.4.0`)
  - Font Awesome (`cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1`)

## Project Structure

```
travo/
├── assets/
│   ├── css/
│   │   ├── _app-6tu7e993jke9dd.css            # Global styles
│   │   └── _app-ge74h44md8sih339.css          # Custom styles for admin panel
│   ├── team/
│   │   └── img/
│   │       └── aryan.webp
│   └── img/
│       ├── ayodhya.png
│       ├── prayagraj.png
│       └── varanasi.png
├── book/                      # /book route
│   ├── ayodhya.html
│   ├── prayagraj.html
│   └── varanasi.html
├── index.html                 # Homepage
├── login.html                 # User login page
├── register.html              # User registeration page
├── forgot-password.html       # Forgot password page
├── reset-password.html        # Reset password page
├── admin.html                 # Admin panel
├── contact.html               # Contact page
├── about.html                 # About Page
├── privacy.html               # Privacy policy
├── terms.html                 # Terms of service
├── favicon.ico                # Favicon
└── README.md                  # This file
```

## Setup Instructions

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, etc.)
- Git installed for cloning the repository
- A local server (e.g., Live Server extension in VS Code or `http-server`) for testing

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/thegitguru/travo.git
   cd travo
   ```

2. **Serve the Application**:
   - Use a local server to run the website. For example, with VS Code's Live Server:
     - Open the project in VS Code.
     - Right-click `index.html` and select "Open with Live Server".
   - Alternatively, use `http-server`:
     ```bash
     npm install -g http-server
     http-server
     ```
     Then navigate to `http://localhost:8080` in your browser.

3. **Access the Admin Panel**:
   - Navigate to `http://localhost:8080/admin.html`.
   - Note: The admin panel includes a simulated authentication check (`isAuthenticated`). For production, implement a real authentication system (e.g., JWT).

### Dependencies
No local installation of dependencies is required, as all libraries (Bootstrap, Chart.js, Font Awesome) are loaded via CDN. Ensure an internet connection for initial testing.

## Usage

- **Homepage (`index.html`)**:
  - Browse travel packages and explore sacred destinations.
  - Sign up or log in to book trips.
  - Subscribe to the newsletter via the footer form.

- **Login (`login.html`)**:
  - Enter credentials to access user features or the admin panel (redirects to `/admin.html` if authorized).

- **Admin Panel (`admin.html`)**:
  - **Dashboard**: View metrics and a user growth chart.
  - **Users**: Search, view, edit, or delete user accounts using the responsive table and modals.
  - **Bookings**: Search, view, or cancel bookings with a responsive table and modals.
  - **Logout**: Redirects to `/login.html` (simulated; replace with backend logout endpoint).
  - **Newsletter**: Subscribe to updates via the footer form (simulated; replace with backend integration).

- **Other Pages**:
  - `contact.html`: Contact form or information.
  - `privacy.html` and `terms.html`: Legal information for users.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and commit:
   ```bash
   git commit -m "Add your feature description"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request on [https://github.com/thegitguru/travo](https://github.com/thegitguru/travo).

Please ensure your code follows the project's coding style and includes appropriate tests.

## Future Enhancements

- **Backend Integration**: Connect to a backend API for real user/bookings data and authentication (e.g., `/api/users`, `/api/bookings`).
- **Additional Charts**: Add pie charts for booking destinations or line charts for trends.
- **Bulk Actions**: Implement checkboxes for bulk delete/cancel in tables.
- **Pagination**: Add pagination for large user/booking lists.
- **Role-Based Access**: Support multiple admin roles with restricted permissions.
- **SEO Improvements**: Enhance meta tags and structured data for better search visibility.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, reach out to [@thegitguru](https://github.com/thegitguru) or open an issue on the repository.

---

*Built with ❤️ for spiritual travelers by [@thegitguru](https://github.com/thegitguru).*
