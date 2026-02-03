# 🚀 Traefik Reverse Proxy Setup with Docker

This project uses **Traefik** as a modern reverse proxy and load balancer to route traffic to multiple Docker services such as APIs, frontends, databases, and admin dashboards.

Traefik automatically detects containers, manages routing, and handles SSL certificates using Let's Encrypt.

---

## 📌 What is Traefik?

Traefik is a **dynamic reverse proxy** designed for container-based environments.  
It provides:

- Automatic routing based on Docker labels  
- HTTPS certificates via Let's Encrypt  
- Load balancing  
- Centralized entrypoint for all services  
- Built‑in dashboard  
- Zero manual configuration when adding new services  

---

## 🧩 Why use Traefik?

### ✔ Route multiple services on one server  
Example:

| Service | URL |
|--------|-----|
| API | https://api.example.com |
| Frontend | https://app.example.com |
| pgAdmin | https://pgadmin.example.com |
| RabbitMQ | https://rabbit.example.com |
| Traefik Dashboard | https://traefik.example.com |

### ✔ No port conflicts  
You no longer expose ports like `3000`, `5050`, `8080`, etc.

### ✔ Automatic SSL  
Traefik generates and renews HTTPS certificates automatically.

### ✔ Auto‑discovery  
When you start a new container with labels, Traefik configures it instantly.

---

## 🛠 Project Structure