# PlacePicker

A modern React application for creating and managing your personal collection of places you'd like to visit or have visited. This project demonstrates advanced React concepts including custom hooks, state management, and API integration.

## Features

- **Browse Available Places**: View a curated collection of scenic locations with images and descriptions
- **Personal Collection**: Add places to your personal wishlist or visited places
- **Interactive UI**: Modern, responsive interface with smooth animations
- **Error Handling**: Robust error handling for network requests and user actions
- **Confirmation Dialogs**: Safe deletion with confirmation modals
- **Loading States**: Visual feedback during data fetching operations

## Tech Stack

### Frontend

- **React 19** - Latest React with modern hooks and features
- **Vite** - Fast build tool and development server
- **Custom Hooks** - Reusable logic for data fetching and state management
- **CSS Modules** - Scoped styling for components

### Backend

- **Node.js** - JavaScript runtime
- **Express.js** - Web framework for API endpoints
- **File-based Storage** - JSON files for data persistence
- **CORS** - Cross-origin resource sharing support

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/vasylpryimakdev/placepicker.git
   cd place-picker
   ```

2. **Install frontend dependencies**

   ```bash
   npm install
   ```

3. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   cd ..
   ```

### Running the Application

1. **Start the backend server**

   ```bash
   cd backend
   npm start
   ```

   The backend will run on `http://localhost:3000`

2. **Start the frontend development server**

   ```bash
   # In a new terminal, from the root directory
   npm run dev
   ```

   The frontend will run on `http://localhost:5173` (default Vite port)

3. **Open your browser**
   Navigate to `http://localhost:5173` to use the application

## API Endpoints

The backend provides the following REST endpoints:

- `GET /places` - Retrieve all available places
- `GET /user-places` - Get user's selected places
- `PUT /user-places` - Update user's place collection

## Project Structure

```
place-picker/
├── public/                 # Static assets
├── src/
│   ├── assets/            # Images and icons
│   ├── components/        # React components
│   │   ├── AvailablePlaces.jsx
│   │   ├── DeleteConfirmation.jsx
│   │   ├── Error.jsx
│   │   ├── Modal.jsx
│   │   ├── Places.jsx
│   │   └── ProgressBar.jsx
│   ├── hooks/             # Custom React hooks
│   │   └── useFetch.js
│   ├── App.jsx            # Main application component
│   ├── http.js            # API utility functions
│   ├── loc.js             # Location utilities
│   └── main.jsx           # Application entry point
├── backend/
│   ├── data/              # JSON data files
│   │   ├── places.json
│   │   └── user-places.json
│   ├── images/            # Place images
│   └── app.js             # Express server
├── package.json
├── vite.config.js
└── index.html
```

## Available Scripts

### Frontend

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Backend

- `npm start` - Start the server with nodemon

## Development

This project is part of a React advanced course, demonstrating:

- Custom hook creation (`useFetch`)
- Optimistic UI updates
- Error boundaries and error handling
- Modal management
- API integration with fetch
- State management patterns

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request