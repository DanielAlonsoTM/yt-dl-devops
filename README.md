# YT-DL-DEVOPS

DevOps repository for the **YT-DL** project.
This repo manages the infrastructure and orchestration of the following submodules:
- [`YT-DL-BACKEND`](https://github.com/DanielAlonsoTM/yt-dl-back) (API service)
- [`YT-DL-FRONT`](https://github.com/DanielAlonsoTM/yt-dl-front) (Frontend application)

---

## 📥 Cloning the Repository with Submodules

### First-time clone (recommended)
```bash
# First-time clone (recommended)
git clone --recurse-submodules https://github.com/<YOUR_USER>/YT-DL-DEVOPS.git
cd YT-DL-DEVOPS
```

### If you already cloned without submodules
```bash
# If you already cloned without submodules
git submodule update --init --recursive
```

### To update submodules later
```bash
git submodule update --remote --merge
```

---

## 🐳 Build and Run with Docker Compose
### Using Docker Hub images
```bash
docker compose -f docker-compose.yml up --build -d
```

### Using local images (builds frontend & backend locally)
```bash
docker compose -f docker-compose-local.yml up --build -d
```
