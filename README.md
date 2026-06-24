

# Zphisher

## Getting Started

### Prerequisites

### Ubuntu Installation

**Step 1 — Open PowerShell as Administrator**

- Press `Win + S`, search for **PowerShell**
- Right-click → **Run as Administrator**
- Click **Yes** on the UAC prompt

**Step 2 — Run the install command**

```powershell
wsl --install
```

This single command will:
- Enable the WSL feature
- Enable the Virtual Machine Platform feature
- Download and install the WSL 2 Linux kernel
- Set WSL 2 as the default version
- Download and install **Ubuntu** (default distro)

**Step 3 — Restart your computer**

```powershell
Restart-Computer
```

After restarting, Launch Ubuntu on search start menu.

### Installation

- Just, Clone this repository -
  ```
  git clone --depth=1 https://github.com/htr-tech/zphisher.git
  ```

- Now go to cloned directory and run `zphisher.sh` -
  ```
  $ cd zphisher
  $ bash zphisher.sh
  ```

- On first launch, It'll install the dependencies and that's it. ***Zphisher*** is installed.

### Manual Tunnel Test

Start Zphisher and choose Localhost (Option 1).  Note the port (e.g., 8080).
In the new terminal:

```
cd zphisher/.server
./cloudflared tunnel -url localhost:8080
```
