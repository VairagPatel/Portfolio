# 🚀 Deploy to Render - Step by Step Guide

## Prerequisites
✅ Your code is pushed to GitHub: https://github.com/VairagPatel/Portfolio
✅ Render configuration files are ready (`render.yaml`, `system.properties`)

## Step-by-Step Deployment

### 1. Create Render Account
- Go to [render.com](https://render.com/)
- Sign up with your GitHub account (recommended)

### 2. Create New Web Service
- Click **"New +"** button in the top right
- Select **"Web Service"**

### 3. Connect GitHub Repository
- Choose **"Build and deploy from a Git repository"**
- Click **"Connect account"** if not already connected
- Find and select: **`VairagPatel/Portfolio`**
- Click **"Connect"**

### 4. Configure Service Settings

**Basic Settings:**
- **Name**: `vairag-portfolio` (or any name you prefer)
- **Region**: Choose closest to your location
- **Branch**: `main`
- **Root Directory**: Leave blank (uses root)

**Build & Deploy:**
- **Environment**: `Docker`
- **Dockerfile Path**: `./Dockerfile` (auto-detected)
- Build and start commands are handled by Dockerfile

**Plan:**
- Select **"Free"** (0$/month, with limitations)
- Or **"Starter"** (7$/month, better performance)

### 5. Environment Variables (Optional)
- **PORT**: `10000` (Render's default, already configured)
- **JAVA_OPTS**: `-Xmx512m` (memory optimization)

### 6. Deploy!
- Click **"Create Web Service"**
- Render will start building your application
- Build process takes 3-5 minutes
- You'll get a live URL like: `https://vairag-portfolio.onrender.com`

## 📋 Build Process
Render will automatically:
1. Clone your GitHub repository
2. Install Java 21
3. Run `mvn clean install -DskipTests`
4. Start the application with the jar file
5. Provide a public HTTPS URL

## 🔄 Auto-Deploy
- Every push to `main` branch will trigger automatic deployment
- No manual intervention needed

## 🐛 Troubleshooting

### Build Fails?
- Check build logs in Render dashboard
- Ensure `pom.xml` is in root directory
- Verify Java version in `system.properties`

### App Won't Start?
- Check application logs
- Verify start command is correct
- Ensure port configuration: `server.port=${PORT:9090}`

### Slow Performance?
- Free tier has limitations (sleeps after 15 min inactivity)
- Consider upgrading to Starter plan
- Optimize Java memory settings

## 📱 Access Your Portfolio
Once deployed, your portfolio will be available at:
`https://your-service-name.onrender.com`

## 🔗 Useful Links
- [Render Dashboard](https://dashboard.render.com/)
- [Render Java Deployment Guide](https://render.com/docs/deploy-spring-boot)
- [Your GitHub Repo](https://github.com/VairagPatel/Portfolio)

---

**Note**: First deployment might take longer. Subsequent deployments are faster due to caching.