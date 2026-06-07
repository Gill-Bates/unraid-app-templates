# Gill-Bates — Unraid Community Apps Templates

Docker app templates for Unraid Community Apps, maintained by Gill-Bates.

---

## 📁 Repository Structure

```
unraid-app-templates/
  README.md
  LICENSE
  .gitignore
  icon.svg
  ca_profile.xml
  templates/
    01_fritzboxinflux.xml
    02_velociraptor.xml
    03_unifi_os_server.xml
  icons/
    01_fritzboxinflux.png
    02_velociraptor.png
    03_unifi_os_server.png
```

- **templates/** — XML templates for each Docker app (one file per app).
- **icons/** — PNG icons referenced in the templates.
- **ca_profile.xml** — Repository profile shown in Community Apps.
- **icon.svg** — Repository icon shown on the maintainer profile page.

---

## 🐳 Apps

| App | Description |
|---|---|
| **fritzinfluxdb** | Pushes Fritz!Box router data to InfluxDB for Grafana dashboards |
| **Velociraptor** | DFIR server with auto-config, multi-arch client repacks and web GUI |
| **UniFi OS Server** | Full UniFi OS stack in Docker (Network App, Identity Hub, PostgreSQL, MongoDB) |

---

## 🧩 Template Format

Each XML file follows Unraid's Docker template specification.
For detailed field reference see the [Community Apps XML Field Reference](https://ca.unraid.net/submit/xml-field-reference).

Key fields per template:

- `<Name>` — Display name in the Unraid Apps section
- `<Repository>` — Docker image reference (e.g. `ghcr.io/user/image:latest`)
- `<Overview>` — Primary summary shown in Community Apps
- `<Icon>` — URL to the app icon (PNG)
- `<TemplateURL>` — Canonical raw URL of this template file
- `<Config>` — Container settings (volumes, ports, environment variables)

---

## 🔗 Submission

This repository is submitted to [Unraid Community Apps](https://ca.unraid.net/submit/new).

Run **Validate** and **Scan** in the submission flow to check all templates before a review request.

---

## 🛠️ Contributing

1. Fork this repository.
2. Add or update templates under `templates/`.
3. Place corresponding icons in `icons/`.
4. Open a pull request with a short description.

**Feature requests or app suggestions?**  
Open an [issue on GitHub](https://github.com/Gill-Bates/unraid-app-templates/issues).

---

## 📜 License

This repository is released under the **MIT License**.  
See [LICENSE](LICENSE) for details.
