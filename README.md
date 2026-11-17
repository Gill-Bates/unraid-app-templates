# Gill-Bates Unraid App Templates

Docker app templates for [Unraid Community Applications](https://ca.unraid.net/), maintained by Gill-Bates.

## Apps

Each template lives in `templates/` and uses the Unraid `Container version="2"` format.

| App | Description | Template | Project | Support |
| --- | --- | --- | --- | --- |
| fritzfluxdb | Collects FRITZ!Box DSL/cable, Wi-Fi, VPN, call, smart-home and router data and sends it to InfluxDB or QuestDB. | [`01_fritzfluxdb.xml`](templates/01_fritzfluxdb.xml) | [Gill-Bates/fritzfluxdb](https://github.com/Gill-Bates/fritzfluxdb) | [Issues](https://github.com/Gill-Bates/fritzfluxdb/issues) |
| velociraptor | Velociraptor DFIR server in Docker (xboarder56 fork), adapted for Unraid. | [`02_velociraptor.xml`](templates/02_velociraptor.xml) | [Xboarder56/velociraptor-docker](https://github.com/Xboarder56/velociraptor-docker) | [Issues](https://github.com/Xboarder56/velociraptor-docker/issues) |
| unifi-os-server | UniFi OS Server in Docker with full systemd-based service management. | [`03_unifi_os_server.xml`](templates/03_unifi_os_server.xml) | [Gill-Bates/unifi-os-server](https://github.com/Gill-Bates/unifi-os-server) | [Unraid forum](https://forums.unraid.net/forum/47-docker-containers/) |
| fetchly | Saves video and audio from YouTube, TikTok, Instagram and Facebook into your own library. | [`04_fetchly.xml`](templates/04_fetchly.xml) | [Gill-Bates/fetchly](https://github.com/Gill-Bates/fetchly) | [Issues](https://github.com/Gill-Bates/fetchly/issues) |
| rct-manager | REST API gateway for RCT Power inverters with an admin GUI. | [`05_rct-manager.xml`](templates/05_rct-manager.xml) | [Gill-Bates/rct-manager](https://github.com/Gill-Bates/rct-manager) | [Issues](https://github.com/Gill-Bates/rct-manager/issues) |
| justup | Self-hosted monitoring of websites, APIs, hosts, TCP/UDP ports and TLS certificates with email or Signal alerts. | [`06_justup.xml`](templates/06_justup.xml) | [Gill-Bates/justup](https://github.com/Gill-Bates/justup) | [Issues](https://github.com/Gill-Bates/justup/issues) |

Descriptions are shortened from the `<Overview>` of each template.

## Installation

### Community Applications

Search for the app name in the **Apps** tab of Unraid and install it from there. The templates are
submitted to [Unraid Community Applications](https://ca.unraid.net/submit/new).

### Manual template URL

1. In the Unraid web UI, open **Docker** and click **Add Container**.
2. Under **Template**, paste the raw URL of the template, for example:

   ```text
   https://raw.githubusercontent.com/Gill-Bates/unraid-app-templates/main/templates/04_fetchly.xml
   ```

3. Review the settings and click **Apply**.

Every template carries its own raw URL in `<TemplateURL>`.

## Repository layout

```text
ca_profile.xml   Maintainer profile shown in Community Applications
templates/       One Unraid template (XML) per app
icons/           PNG icon per app (<Icon> in the templates) and the profile icon gill-bates.png
LICENSE          MIT License
```

## Template conventions

- Files are named `NN_<app>.xml` and set `<TemplateURL>` to their own raw URL on `main`.
- `<Icon>` points to a PNG in `icons/` through a raw URL on `main`.
- `<Project>` and `<Support>` link to the upstream project and its issue tracker or forum.
- Field reference: [Community Apps XML Field Reference](https://ca.unraid.net/submit/xml-field-reference).
- Reference repository for structure and conventions: [Portabase/unraid-templates](https://github.com/Portabase/unraid-templates).

Before requesting a review, run **Validate** and **Scan** in the Community Applications submission flow.

## License

Released under the [MIT License](LICENSE).

<br>
<p align="center">
  <a href="https://www.buymeacoffee.com/tnsteinerx">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy%20me%20a%20beer&emoji=%F0%9F%8D%BA&slug=tnsteinerx&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" alt="Buy Me A Coffee">
  </a>
</p>