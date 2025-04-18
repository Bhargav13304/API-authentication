# 🔐 API Authentication - Secure Login App

**API Authentication** is a Node.js-based backend project implementing authentication logic using Express.js. It supports user login via hardcoded credentials and serves secure views using EJS templates. This is ideal for understanding basic backend authentication flow without database integration.

---

### 💡 Technologies Used, Applications & Advantages

- **Node.js** – Backend runtime for scalable JavaScript applications.
- **Express.js** – Routing and server management made easy.
- **EJS (Embedded JavaScript Templates)** – Dynamic rendering of HTML based on logic.
- **Body-parser** – Parses incoming form data from POST requests.

**Applications:**
- Authentication flow prototype
- Learning user login and session validation
- Lightweight credential-based login system

**Advantages:**
- Extremely simple for quick learning
- No external DB dependencies
- Clean login routing with form handling

---

### 📦 Installation & Running the App

```bash
# Clone the repository
git clone https://github.com/Bhargav13304/API-authentication.git
cd API-authentication

# Install dependencies
npm install

# Run the server
node solution.js
```

Open your browser and navigate to `http://localhost:3000` to access the login page.

---

### 📁 Project Structure

```
API-authentication/
├── views/
│   ├── index.ejs          # Login form UI
│   └── secret.ejs         # Protected page shown after successful login
├── solution.js            # Express server and login logic
├── package.json           # Project metadata and dependencies
└── README.md              # Documentation
```

---


