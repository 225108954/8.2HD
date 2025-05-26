## 🐳 How to Run the Dockerised Container

Follow the instructions below to build and run this application inside a Docker container for assessment.

---

### 🛠️ Build the Docker Image

Make sure you're in the root directory of the project and Docker is installed and running.

```bash
docker build -t splitdeal-app .
```

> This command builds the Docker image using the Dockerfile in the root folder.

---

### 🚀 Run the Container

You must provide a `.env` file with all required environment variables like `MONGODB_URI`, `JWT_SECRET`, etc.

```bash
docker run -p 3000:3000 --env-file .env splitdeal-app
```

> This exposes the app on your local machine at `http://localhost:3000`.

---

### 🌐 Access the Application

- App home page:  
  [http://localhost:3000](http://localhost:3000)

- Student Identity Route:  
  [http://localhost:3000/api/student](http://localhost:3000/api/student)

---

### 📦 Example Output of `/api/student`

```json
{
  "name": "Gaurav Myana",
  "studentId": "225108954"
}
```



