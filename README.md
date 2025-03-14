# DarkRepoLauncher

DarkRepoLauncher is an "autolauncher" for DARK REPO C# Mono Cheat.

## Features

- **Secure Downloads:**  
  Downloads files securely over TLS using Rust's reqwest crate.
- **File Integrity:**  
  Verifies files with SHA256 hashes.
- **APPDATA Storage:**  
  Stores all files in your APPDATA folder.
- **Auto-Update:**  
  Automatically fetches the latest release from GitHub.
- **Process Injection:**  
  Waits for the target process and injects the DLL via SharpMonoInjector.
- **Admin Check:**  
  Auto-elevates if not run as administrator.

## Installation & Usage

1. **Clone & Build:**
   ```bash
   git clone https://github.com/hdunl/DarkRepoLauncher.git
   cd DarkRepoLauncher
   cargo build --release
   ```
   
**Run as Administrator**: Launch the executable. It will request elevation if needed.

**Start**: Press Enter to begin. The launcher downloads and verifies files, waits for the target process, and then injects the DLL.
