# 🧠 GraphQL Job Board – Server

This is the **GraphQL backend server** for the Job Board App, built with **Apollo Server** and **Node.js**. It serves job listings, company info, and related queries for a client-side React app.

---

## 🚀 Features
- GraphQL schema for jobs and companies
- Resolvers to handle queries and mutations
- In-memory or mock data setup for development
- Clean modular folder structure

---

## 🛠 Tech Stack
- Node.js
- Apollo Server
- GraphQL

---

## 📁 Project Structure
```
├── index.js         # Entry point
├── schema.js        # GraphQL type definitions
├── resolvers.js     # Query/Mutation resolvers
├── db.js            # Mock data source
└── package.json
```

---

## ▶️ Running Locally
```bash
npm install
npm start
```

GraphQL Playground will be available at: `http://localhost:4000/`

---

## 🔍 Sample Queries
```graphql
query {
  jobs {
    id
    title
    company {
      name
    }
  }
}

mutation {
  createJob(input: { title: "Frontend Developer", companyId: "c1" }) {
    id
    title
  }
}
```

---

## 📄 License
Open source under the [MIT License](LICENSE).
