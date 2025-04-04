## 🌟 **Frontend Developer Challenge – Recipe Galaxy!** 🍽️🌐  
**Monthly Challenge – April 2025**

> Design a gorgeous, functional, and interactive UI for the Recipe Galaxy backend. Use modern tools. Focus on user experience. ✨

---

### 🎯 **Objective**
Build a responsive **Recipe Web App** using **React + TailwindCSS** (or any modern frontend stack). Connect it to the Recipe Galaxy API (or mock your own) and show off your frontend wizardry with **beautiful UI, solid code, and great UX**.

---

### 🧠 **What You'll Be Judged On**
- Clean & componentized architecture
- Use of **TailwindCSS** & utility-first design
- Pagination, filtering & search UX
- API integration & state management
- Code quality, reusability & performance
- Deployment, testing & documentation
- Git hygiene & commit structure

---

### 🧾 **Core Features**

#### 🧁 1. Recipe List View
- Fetch and display list of recipes (from `/recipes`)
- Show:
  - Title
  - Prep Time
  - Difficulty (badge-style UI)
  - Short preview or image (optional)
- Add:
  - Search (`?search=`)
  - Filter (`?difficulty=&maxPrepTime=`)
  - Pagination (`?page=1&limit=6`)
- Use **loading skeletons** and **error states**

---

#### 🍲 2. Recipe Details Page
- Show full recipe:
  - Title
  - Ingredients (styled list)
  - Instructions (nicely formatted)
  - Prep time & difficulty
- UI should be elegant and responsive

---

#### ➕ 3. Add Recipe Form (Bonus 🔥)
- Form with:
  - Title, Ingredients (dynamic input), Instructions, Difficulty, Prep Time
- Add client-side validation
- Use toasts/snackbars for feedback
- Post to `/recipes`

---

#### 📊 4. Stats Page (Optional)
Fetch from `/recipes/stats` and show:
- Total recipes
- Average prep time
- Count by difficulty (with bar chart using `recharts`, `chart.js`, etc.)

---

### 🧱 Tech Stack (Recommended)
Use **React + TailwindCSS** and optionally combine with:

#### 🧰 Core
- ⚛️ `React` (or `Next.js`)
- 🎨 `TailwindCSS` (with `@tailwind/forms`, `@tailwind/typography`)
- 🌐 `axios` or `fetch`
- 🔀 `react-router-dom` for routing
- 🔄 `react-query` / `swr` for data fetching & caching
- 📦 `clsx` for conditional classNames

#### 🧠 Optional UI Libraries
- 🧱 `shadcn/ui` – modern components with Tailwind
- 🧩 `Headless UI` – accessible dropdowns/modals
- 🪄 `Radix UI` – primitives for tooltips, sliders, etc.
- 💡 `Lucide` for icons

---

### ✅ Testing
- 🧪 Unit tests with `Vitest` or `Jest`
- 🧼 Test component rendering & form validation
- 🚦 Optional: E2E tests with `Cypress`

---

### 🧘 Folder Structure (Recommended)
```
/src
  /components   -> UI components (Card, Button, Input)
  /pages        -> Route-based views
  /api          -> API wrappers (axios/fetch)
  /hooks        -> Custom hooks (useRecipes, usePagination)
  /types        -> Type definitions
  /assets       -> Icons, images
```

---

### 📘 README.md Checklist
- 📦 Tech stack used
- 📂 Folder structure
- 🔌 How to run the app locally
- 🧪 How to run tests
- 🌐 Live demo link (Vercel/Netlify/etc.)
- 🧠 API notes (if mocked)

---

### 🧪 Example API Usage
```bash
# Get 5 recipes, filtered
curl http://localhost:3000/recipes?difficulty=easy&maxPrepTime=20&search=pasta&page=1&limit=5
```

---

### 🚀 Bonus Features (Optional But Impressive)
- 🌒 Dark mode toggle
- ❤️ Like or bookmark recipes
- 📸 Upload image preview (Multer + Cloudinary or just a local preview)
- 📦 Offline caching (service workers)
- 🔑 Auth for adding/editing recipes (Firebase Auth, etc.)

---

### 🐙 Submission Rules
- Push code to **public GitHub repo**
- Follow **conventional commits**
- Open an issue in the challenge repo with the tag `#RecipeFrontend`
- Mention `@theakshaydhiman` for review
- Live deployment link (Netlify, Vercel, etc.) = Bonus ✨

---

### ✅ Example Commit Messages
```
feat: add recipe list with search and filters
feat: implement recipe detail page
fix: handle empty API responses
docs: update README with setup instructions
```
