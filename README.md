# Portfolio - Vairag Akbari

A modern, responsive personal portfolio website built with Spring Boot and Thymeleaf.

## 🚀 Features

- **Responsive Design** - Works seamlessly on all devices
- **Modern UI** - Clean and professional interface
- **Dynamic Sections**:
  - Hero section with social links
  - About me with skills showcase
  - Projects portfolio
  - Experience timeline
  - Certifications
  - Achievements
  - Contact form

## 🛠️ Tech Stack

- **Backend**: Spring Boot 3.5.0
- **Frontend**: HTML5, CSS3, JavaScript
- **Template Engine**: Thymeleaf
- **Build Tool**: Maven
- **Java Version**: 21

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/VairagPatel/Portfolio.git
cd Portfolio
```

2. Build the project:
```bash
mvn clean install
```

3. Run the application:
```bash
mvn spring-boot:run
```

4. Open your browser and navigate to:
```
http://localhost:9090
```

## 🌐 Deployment

### Render Deployment

1. Push your code to GitHub
2. Go to [Render Dashboard](https://dashboard.render.com/)
3. Click "New +" → "Web Service"
4. Connect your GitHub repository: `VairagPatel/Portfolio`
5. Configure the service:
   - **Name**: `vairag-portfolio`
   - **Environment**: `Java`
   - **Build Command**: `mvn clean install -DskipTests`
   - **Start Command**: `java -jar target/personalportfolio-0.0.1-SNAPSHOT.jar`
6. Deploy!

### Railway Deployment (Alternative)

1. Push your code to GitHub
2. Connect your GitHub repository to Railway
3. Railway will auto-detect the Spring Boot application
4. Set the following environment variables (if needed):
   - `PORT`: 9090 (or Railway's default)
5. Deploy!

## 📝 Configuration

The application runs on port 9090 by default. You can change this in `application.properties`:

```properties
server.port=9090
```

## 👤 About Me

- **Name**: Vairag Akbari
- **Education**: B.Tech in Computer Science, Vellore Institute of Technology, Bhopal
- **CGPA**: 8.34
- **Email**: vairag.techwork@gmail.com
- **LinkedIn**: [linkedin.com/in/vairagakbari](https://linkedin.com/in/vairagakbari)
- **GitHub**: [github.com/VairagPatel](https://github.com/VairagPatel)
- **LeetCode**: [leetcode.com/u/Vairag0310](https://leetcode.com/u/Vairag0310/)

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

---

Made with ❤️ by Vairag Akbari
