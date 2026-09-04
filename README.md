# 🚀 CoreMTARG - Custom MTA:SA Server Package

CoreMTARG is a custom Multi Theft Auto RG: San Andreas (MTARG:SA) server build pre-configured with custom x64 binaries, custom resources, and dedicated launcher backend support.

This repository contains the full server deployment package and a custom **Pterodactyl Egg** for automated setup and deployment.

---

## 📋 Prerequisites

* **Pterodactyl Game Panel** (v1.x or higher)
* **Required Network Ports:**
  * `Game Port`: Default `22003` (UDP)
  * `HTTP Port`: Default `22005` (TCP)
  * `ASE Port`: Default `22004` (UDP)

---

## 🛠️ Step-by-Step Pterodactyl Installation Guide

### Step 1: Import the Custom Egg
1. Log in to your Pterodactyl **Admin Control Panel**.
2. Navigate to **Nests** in the left sidebar.
3. Click the **Import Egg** button at the top right.
4. Upload the `egg-coremtarg.json` file from this repository and assign it to a Nest (e.g., GTA Nests).

### Step 2: Create the Server
1. Go to **Servers > Create New**.
2. Set the Server Name, Owner, and Node.
3. Under **Nest & Egg Selection**:
   * Select your imported **Nest**.
   * Choose **CoreMTARG Custom Server** as the Egg.
4. Set the allocations/ports and click **Create Server**.

### Step 3: Install & Start the Server
1. Open the created server in the **User Console**.
2. Go to **Settings > Reinstall Server** (This automatically downloads and extracts the latest `coremtarg.zip` from GitHub Releases).
3. Once the installation script finishes, click **Start**.

---

## ⚙️ Server Configuration

To modify your server settings, navigate to the `mods/deathmatch/` directory:

* **`mtaserver.conf`**: Configure Server Name, Max Players, Web/HTTP Ports, and Passwords.
* **`acl.xml`**: Manage Admin permissions and resource access control lists.

---

## 🔧 Features Included

* **Optimized x64 Binaries:** Pre-configured 64-bit Linux support with custom shared libraries.
* **Auto Permission Handler:** Executable permissions (`chmod +x`) are automatically set for `mta-server64` and `x64/` modules during setup and startup.
* **Launcher Ready:** Compatible with custom MTA client launcher backends out of the box.

---

## 📞 Support & Issues

If you encounter any bugs or need assistance during installation, please open an issue:
* **GitHub Issues:** [Create an Issue](https://github.com/mtarg/mtarg-linux-ubuntu-files/issues)
