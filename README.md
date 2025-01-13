# Unraid Community App Template for Bolt DIY

This repository provides a **Community App Template** for Unraid to easily deploy the [Bolt DIY](https://github.com/stackblitz-labs/bolt.diy) Docker container. Bolt is a lightweight, open-source framework for building and running web applications and APIs. The DIY version allows for custom configurations and extensions.

## Features
- Easy installation via Unraid's Community Apps.
- Pre-configured ports, volumes, and environment variables.
- Customizable timezone (default: `Europe/Berlin`).
- Persistent storage for application data.

## How to Use
1. **Add the Template to Unraid:**
   - Go to the **Apps** tab in Unraid.
   - Click on **Install**.
   - Paste the following URL:
     ```
     https://raw.githubusercontent.com/Eth030/unraid-bolt-diy-template/main/template.xml
     ```
   - Click **Install**.

2. **Configure the Container:**
   - Set the host port (default: `8181`).
   - Adjust the timezone if needed (default: `Europe/Berlin`).
   - Specify the data storage location (default: `/mnt/user/appdata/boltdiy`).

3. **Start the Container:**
   - Launch the container from the Unraid interface.
   - Access the web interface at `http://[YOUR_UNRAID_IP]:8181`.

## Template Details
- **Repository:** `ghcr.io/stackblitz-labs/bolt.diy:latest`
- **WebUI Port:** `8181` (host) → `80` (container)
- **Timezone:** `Europe/Berlin` (customizable)
- **Data Volume:** `/mnt/user/appdata/boltdiy` → `/app/data`

## Support
For issues or questions:
- Open an issue in this repository.
- Visit the [Bolt DIY GitHub repository](https://github.com/stackblitz-labs/bolt.diy).

## License
MIT License. See [LICENSE](LICENSE) for details.
