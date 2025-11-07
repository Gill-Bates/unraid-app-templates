# Unraid Community Apps Repository

This repository contains **custom Unraid Community App templates** for easy installation and management of Docker containers through the Unraid web interface.

---

## 📁 Repository Structure

```
/community-apps/
├── appname.xml           # Template definition for an Unraid app
├── anotherapp.xml
/icons/
└── appname.png           # Icon used in the Unraid UI
└── anotherapp.png        # Icon used in the Unraid UI
```

- **community-apps/** — contains all XML templates.  
- **icons/** — contains PNG icons referenced in the templates.


---

## 🧩 Template Format

Each XML file follows Unraid’s template specification:

- `Name`: Display name shown in the Unraid Apps section.  
- `Repository`: Docker image reference (e.g. `ghcr.io/user/image:latest`).  
- `WebUI`: URL for accessing the app’s web interface.  
- `Icon`: Path to a 128×128 PNG icon (e.g. `/icons/appname.png`).  
- `Config` entries define container settings like volumes, ports, and environment variables.

For detailed reference, see the [Unraid Template Documentation](https://wiki.unraid.net/Development/Creating_Your_Own_Templates).

---

## 🛠️ Contributing

1. Fork this repository.  
2. Add or update templates under `/community-apps/`.  
3. Place corresponding icons in `/icons/`.  
4. Open a pull request with a short and clear description.

---

## 📜 License

This repository is released under the **MIT License**.  
Feel free to use, modify, and distribute the templates for your own Unraid setup.
