## 🌟 **Backend Developer Challenge – Recipe Galaxy!** 🌍🍳  
**Monthly Challenge – April 2025**

### 👨‍🍳 Build a Deliciously Scalable Recipe API – Your Way!

---

### 🎯 **Objective**
Design and implement a **Recipe Management API** using *any backend technology you love* (Node.js, Django, FastAPI, Go, etc.).

Your mission: Build a high-performance, developer-friendly, and feature-rich backend that powers the **ultimate recipe sharing app**. Focus on real-world features like caching, filtering, pagination, clean architecture, and testing. Bonus if it’s Dockerized & well-documented!

---

### 🧠 **What You'll Be Judged On**
- REST API design and structure
- Code quality, modularity & readability
- Real-world features: pagination, filtering, etc.
- Redis caching strategy
- Testing strategy & coverage
- Git hygiene & commit structure
- Documentation quality
- Bonus points for Docker support and deploy readiness

---

### 🧾 **Feature Requirements**

#### 📦 1. Recipe Model
Each recipe should include:
- `title`: string (required)
- `ingredients`: array of strings (required)
- `instructions`: rich text or plain string (required)
- `difficulty`: one of `easy`, `medium`, `hard`
- `prepTime`: number (in minutes)
- `createdAt`: timestamp (default now)

👉 Add **validation rules** & **defaults** based on your stack.

---

#### ⚙️ 2. RESTful API Endpoints
Design the following routes:
- `GET /recipes` – list all recipes
- `POST /recipes` – create a new recipe
- `GET /recipes/:id` – fetch a single recipe
- `PUT /recipes/:id` – update a recipe
- `DELETE /recipes/:id` – delete a recipe

🔧 Bonus Route:
- `GET /recipes/stats` – returns:
  - total recipe count
  - average prep time
  - recipe count per difficulty

---

#### 🔍 3. Pagination, Filtering & Search
Your `GET /recipes` endpoint should support:
- Pagination: `?page=1&limit=10`
- Search by title: `?search=pasta`
- Filter by difficulty and max prep time:  
  `?difficulty=easy&maxPrepTime=30`

---

#### ⚡ 4. Redis Caching
Use **Redis** to cache:
- Individual recipe fetches (`/recipes/:id`)
- Popular search queries with pagination

⏱️ Set a cache TTL (e.g. 1 hour)  
♻️ Invalidate cache on updates or deletions

---

#### 🔐 5. Environment Configuration
- Use `.env` or your stack’s config strategy
- Secrets like DB URLs, Redis host, ports, etc., must be configurable

---

#### ✅ 6. Testing Suite
Write **unit & integration tests** using your preferred framework:
- Test model validations
- Test API responses & status codes
- Test Redis caching logic (mock Redis if needed)

📈 Aim for **80%+ coverage**

---

#### 🧹 7. Code Quality
- Follow best practices of your chosen language
- Use a linter (`ESLint`, `flake8`, `golangci-lint`, etc.)
- Modular folder structure (routes, controllers, services, etc.)
- Use Prettier or formatter to keep the code tidy

---

#### 🐳 8. Docker & Docker Compose (Bonus)
Add a `Dockerfile` and `docker-compose.yml`:
- App service
- DB (MongoDB/PostgreSQL/MySQL)
- Redis

🧪 Optional: Add a service for running tests!

---

#### 📘 9. README.md
Your documentation should include:
- 📦 Project setup (manual + Docker)
- 🔌 API reference with curl examples
- ⚙️ How caching works
- 🧪 How to run tests
- 🙌 Contribution guide

Make it clean, beginner-friendly, and stylish!

---

#### 🐙 10. Git & Repo Hygiene
- Follow **conventional commit** messages:
  - `feat: add recipe stats endpoint`
  - `fix: correct pagination logic`
  - `docs: update README with API usage`
- Push your code to a **public GitHub repo**
- Keep your commits small & meaningful

---

### 📡 **Sample API Requests**
```bash
# Get first 5 recipes
curl http://localhost:3000/recipes?page=1&limit=5

# Search recipes by keyword
curl http://localhost:3000/recipes?search=chicken

# Filter by difficulty and max prep time
curl http://localhost:3000/recipes?difficulty=easy&maxPrepTime=20
```

---

### 💥 **Bonus Features (Optional but Impressive)**
- ✅ User Auth (JWT or OAuth) and recipe ownership
- ⭐ Like/favorite recipes
- 📝 User comments or ratings
- 📸 Image upload support (Multer, Cloudinary, S3, etc.)
- 🌍 Deploy to Render/Heroku/Vercel/AWS

---

### 🚀 Submission Guidelines
- Create a GitHub repo (e.g., `Recipe-Galaxy-April`)
- Complete your project
- Open an issue in our challenge repo with the tag `#RecipeBackend`
- Mention `@jobcodeteam` for review
- Share your repo link (must be public)

