## Getting Started

### Prerequisites

- **Node.js** (v14 or higher recommended)
- **npm** (comes with Node.js)
- **MongoDB** (local or Atlas)
- **Redis** (see below for Windows instructions)

---

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

---

### 2. Install Dependencies

```bash
npm install
```

---

### 3. Setup MongoDB

- **Local MongoDB:**  
  Make sure MongoDB is running locally.  
  Example URI:

  ```
  mongodb://127.0.0.1:27017/your-db-name
  ```

- **MongoDB Atlas:**  
  Get your connection string from [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).

- **Configure the URI:**  
  Edit `config/keys.js` and set your `mongoURI`:
  ```js
  module.exports = {
    mongoURI: "your-mongodb-uri-here",
    cookieKey: "your-cookie-key"
  };
  ```
  Or, set the `MONGO_URI` environment variable.

---

### 4. Install and Run Redis on Windows

#### Option 1: Using Memurai (Recommended for Windows)

1. Download Memurai Community Edition from [https://www.memurai.com/get-memurai](https://www.memurai.com/get-memurai)
2. Install and run Memurai (it works just like Redis).

#### Option 2: Using Redis with WSL (Windows Subsystem for Linux)

1. Install [WSL](https://docs.microsoft.com/en-us/windows/wsl/install)
2. Open your WSL terminal and run:
   ```bash
   sudo apt update
   sudo apt install redis-server
   redis-server
   ```

#### Option 3: Using Redis Windows Port (Unofficial, not recommended for production)

1. Download from [https://github.com/microsoftarchive/redis/releases](https://github.com/microsoftarchive/redis/releases)
2. Extract and run `redis-server.exe`

---

### 5. Start the Application

```bash
npm run dev
```

The server will start on [http://localhost:5000](http://localhost:5000).

---

### Troubleshooting

- **MongoDB URI malformed:**  
  Double-check your `mongoURI` in `config/keys.js` or your environment variable.
- **Redis not running:**  
  Make sure Redis/Memurai is running before starting the app.

---

## Bonus!

Interested in some of my other courses? Try one out now!

- [Rust: The Complete Developer's Guide](https://www.udemy.com/course/rust-the-complete-developers-guide/?couponCode=7962AD119BE43DCBF7AC)
- [Next JS: The Complete Developer's Guide](https://www.udemy.com/course/next-js-the-complete-developers-guide/?couponCode=FE4F82A0F03262F678AC)
- [ChatGPT and LangChain: The Complete Developer's Masterclass](https://www.udemy.com/course/chatgpt-and-langchain-the-complete-developers-masterclass/?couponCode=4CCDA21198171837F008)
- [React Testing Library and Jest: The Complete Guide](https://www.udemy.com/course/react-testing-library-and-jest/?couponCode=55EDF3F82495355A23AD)
- [Redis: The Complete Developer's Guide](https://www.udemy.com/course/redis-the-complete-developers-guide-p/?couponCode=5ED356122C0B4D676FEC)
- [SQL and PostgreSQL: The Complete Developer's Guide](https://www.udemy.com/course/sql-and-postgresql/?couponCode=983CEA231DA59F4596C2)
- [Docker and Kubernetes: The Complete Guide](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/?couponCode=390956E5AE3795A0E0F3)
- [NestJS: The Complete Developer's Guide](https://www.udemy.com/course/nestjs-the-complete-developers-guide/?couponCode=3E3B5E71C411F773E9DB)
- [Microservices with Node JS and React](https://www.udemy.com/course/microservices-with-node-js-and-react/?couponCode=DAA62568E8CEBC5F74F1)
- [Microfrontends with React: A Complete Developer’s Guide](https://www.udemy.com/course/microfrontend-course/?couponCode=018241672B52C470ECC3)
- [Go: The Complete Developer's Guide (Golang)](https://www.udemy.com/course/go-the-complete-developers-guide/?couponCode=A540E048F7FFAF58FEF3)
- [Typescript: The Complete Developer's Guide](https://www.udemy.com/course/typescript-the-complete-developers-guide/?couponCode=9E1C31304E4A51679D9F)
- [Modern React with Redux [2024 Update]](https://www.udemy.com/course/react-redux/?couponCode=DF9A5A554EFFDB4B85DB)
