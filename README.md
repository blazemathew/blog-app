# Blog Application

A modern blog application built with Angular that supports social authentication, post management, and real-time updates.

## Features

- 🔐 Social Authentication (Google & Facebook)
- 📝 Create, Read, Update, Delete (CRUD) operations for blog posts
- 🎨 Modern and responsive UI
- 🔒 Protected routes with Auth Guard
- 🔄 Auto token refresh mechanism
- 📱 Mobile-friendly design

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js (v16 or higher)
- npm (v8 or higher)
- Angular CLI (v17 or higher)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/blog-application.git
cd blog-application
```

2. Install dependencies:
```bash
npm install
```

3. Configure environment variables:
   - Copy `src/environments/environment.example.ts` to `src/environments/environment.ts`
   - Update the `apiUrl` and other configuration values as needed

## Development Server

Run the development server:

```bash
ng serve
```

Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Project Structure

```
src/
├── app/
│   ├── components/           # Application components
│   │   ├── auth-callback/    # OAuth callback handling
│   │   ├── dashboard/        # Main dashboard view
│   │   ├── login/           # Login component
│   │   ├── post-detail/     # Post viewing component
│   │   ├── post-list/       # Post listing component
│   │   └── create-post/     # Post creation component
│   ├── core/                # Core functionality
│   │   ├── guards/          # Route guards
│   │   ├── interfaces/      # TypeScript interfaces
│   │   ├── services/        # Application services
│   │   └── interceptors/    # HTTP interceptors
│   └── environments/        # Environment configurations
```

## Features in Detail

### Authentication
- Social login support (Google, Facebook)
- JWT-based authentication
- Automatic token refresh
- Protected routes with Auth Guard

### Post Management
- Create new blog posts
- View post details
- Edit existing posts
- Delete posts
- List view of all posts

### Security Features
- JWT Interceptor for authenticated requests
- Secure route protection
- Token refresh mechanism
- XSS protection

## Building for Production

To build the project for production:

```bash
ng build
```

The build artifacts will be stored in the `dist/` directory.

## Running Tests

Execute unit tests via Karma:

```bash
ng test
```

Run end-to-end tests:

```bash
ng e2e
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Dependencies

- @angular/core
- @angular/common
- @angular/router
- @angular/forms
- @angular/platform-browser
- @angular/animations

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.