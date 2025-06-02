# 🚀 Laravel 12 + PHP 8.3 Docker Template  
> **Modern Laravel Starter Kit** with **FilamentPHP**, **WebSockets (Soketi)**, **Redis**, **MySQL**, **PostgreSQL** and clean Docker setup.

---

## 🌟 Key Features

✅ **Laravel 12** with **PHP 8.3** (latest stable)  
✅ **Laravel Queue** with Redis  
✅ **FilamentPHP v3** – Admin panel made simple  
✅ **Soketi** – Self-hosted WebSocket server (Pusher-compatible)  
✅ **Redis** – Queue & caching  
✅ **MySQL 5.7** – Legacy-compatible relational DB  
✅ **PostgreSQL 15** – Advanced relational DB support  
✅ **Node.js 18 LTS** – Asset compilation  
✅ **Supervisor** – Process control for queues and services  
✅ **Nginx** – Production-grade web server  
✅ **Multi-stage Dockerfile** – Optimized for performance  
✅ **Windows-friendly** – Fixes line-endings, safe git directory  
✅ **Flexible ENV support** – Auto-loads `.env.${APP_ENV}`  
✅ **CI/CD Ready** – Extendable for GitHub Actions, Jenkins, etc.

---

## ⚙️ Setup Instructions

### 1. Clone and prepare the environment
```bash
git clone https://github.com/ShaonMajumder/docker-template_laravel-12-php-8.3-npm-mysql-redis-nginx-queue-soketi.git laravel-docker-starter
cd laravel-docker-starter
docker-compose --env-file environment/.env.local up --build
```

## 🌐 Access Points

| Service      | URL                         | Description              |
|--------------|-----------------------------|--------------------------|
| App          | http://localhost:8000       | Laravel Frontend         |
| Filament     | http://localhost:8000/admin | Admin Panel              |
| Soketi       | ws://localhost:6001         | WebSocket Server         |
| MySQL        | localhost:3306              | MySQL DB (root/root)     |
| Redis        | localhost:6379              | Redis Instance           |

---

## 🧰 Developer Notes

- Modify startup behavior in `docker/startup.sh`.
- Windows compatibility via `dos2unix` and Git safe.directory.
- Socket event broadcasting is ready with Laravel + Soketi + Redis.
- Customize Nginx in `docker/nginx/default.conf`.

---

## 🛡️ Security & Scaling Tips

- Use HTTPS (reverse proxy or Let's Encrypt via Traefik/Nginx).
- Scale `queue` and `soketi` services using Docker Swarm or Kubernetes.
- Enable JWT authentication for APIs and WebSockets.
- Use Laravel Horizon for queue monitoring.
- Add Prometheus/Grafana for observability.

---

## 🧠 Why this Boilerplate?

This setup is ideal for:

- **Senior Developers** needing a clean microservice-ready stack.
- **Startups** launching quickly with admin dashboards (Filament).
- **Job Candidates** showing DevOps and backend skills.
- **Hackathon Teams** shipping fast with real-time features.

---

## 📜 License

MIT – use freely, contribute respectfully.

---

## 👨‍💻 Maintainer

**Shaon Majumder**  
Senior Software Engineer | [robist.com](https://robist.com)  
🔧 Backend Specialist | 💬 System Designer | 🧠 OSS Contributor  
🔗 [LinkedIn](https://linkedin.com/in/shaonmajumder) | [GitHub](https://github.com/shaonmajumder)
