<h1 align="center">SDO Keystone</h1>

<p align="center">The Admin app for Sound Doctrine Online powered by Keystone JS.</p>

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- PostgreSQL database

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sounddoctrine-de/sdo-keystone.git
   cd sdo-keystone
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory with the following variables:
   ```env
   KEYSTONE_DB_URL=postgresql://username:password@localhost:5432/sdo_keystone
   KEYSTONE_SESSION_SECRET=your-session-secret-here
   ```

### Running the Application

#### Development Mode

To start the development server:

```bash
npm run dev
```

The Keystone admin interface will be available at `http://localhost:3000`

#### Production Mode

1. Build the application:
   ```bash
   npm run build
   ```

2. Start the production server:
   ```bash
   npm start
   ```

### Database Setup

Before running the application, make sure your PostgreSQL database is set up and accessible with the connection string provided in your `.env` file.

The application will automatically handle database migrations and schema updates through Keystone's built-in migration system.
