# 🔐 API Authentication - Secure Login App

**API Authentication** is a Node.js-based backend project that implements authentication logic using Express.js and integrates a PostgreSQL database to validate user credentials. It renders login forms with EJS templates and processes login requests securely. This app is perfect for understanding backend auth logic with a real database connection.

---

### 💡 Technologies Used, Applications & Advantages

- **Node.js** – JavaScript runtime for scalable backend development.
- **Express.js** – Minimalist web framework for handling routes and requests.
- **EJS (Embedded JavaScript Templates)** – Server-side HTML rendering.
- **Body-parser** – Parses incoming request bodies.
- **PostgreSQL** – SQL database used to store and validate user credentials.
- **pg (node-postgres)** – PostgreSQL client for Node.js.

**Applications:**
- Secure login systems with real database support
- Learning full-stack authentication workflow
- Lightweight starter backend for auth-enabled apps

**Advantages:**
- Integrates real-world login validation with PostgreSQL
- Minimalistic yet extendable
- Teaches basic data handling, querying, and secure rendering

---

### 📦 Installation & Running the App

```bash
# Clone the repository
git clone https://github.com/Bhargav13304/API-authentication.git
cd API-authentication

# Install dependencies
npm install
```

> Make sure PostgreSQL is installed and running.

1. **Set up PostgreSQL user table:**
   - Connect to your PostgreSQL client (e.g., `psql`, DBeaver, pgAdmin).
   - Create a database (e.g., `authdb`) and a `users` table:

   ```sql
   CREATE TABLE users (
     username VARCHAR(255),
     password VARCHAR(255)
   );

   INSERT INTO users (username, password) VALUES ('admin', 'admin123');
   ```

2. **Configure database connection:**
   - Update your `solution.js` with your PostgreSQL credentials:

   ```js
   const client = new Client({
     user: 'your_username',
     host: 'localhost',
     database: 'authdb',
     password: 'your_password',
     port: 5432
   });
   ```

3. **Run the server:**

```bash
node solution.js
```

> Navigate to `http://localhost:3000` to use the login form.

---

### 📁 Project Structure

```
API-authentication/
├── views/
│   ├── index.ejs          # Login form UI
│   └── secret.ejs         # Protected page after successful login
├── solution.js            # Main Express app with PostgreSQL connection
├── package.json           # Dependencies
└── README.md              # Project documentation
```

---


