<h1>🛡️ proxy-lab.sh - Two Blockers, One Scripted Solution</h1>

<p align="center">
  <a href="https://github.com/Udantha4748/proxy-lab.sh" style="display:inline-block;padding:16px 32px;background:linear-gradient(135deg,#667eea 0%,#764ba2 100%);color:#ffffff;font-size:20px;font-weight:bold;border-radius:50px;text-decoration:none;box-shadow:0 4px 15px rgba(102,126,234,0.4);">⬇️ Download proxy-lab.sh</a>
</p>

## 🎯 What Is proxy-lab.sh?

proxy-lab.sh is a smart automation tool that fixes two common Android networking problems — device trust issues and proxy routing failures — in one simple script. It checks your setup before running, catches common mistakes early, and works on both Android emulators and iOS simulators. Think of it as a friendly mechanic that inspects your car before taking it for a spin, so you don't break down halfway.

## 🚀 Getting Started

Getting started with proxy-lab.sh takes less than five minutes. No coding experience needed. No complicated commands to memorize. Just follow these simple steps.

### Step 1: Visit the Download Page

Visit this link to download the application: [https://github.com/Udantha4748/proxy-lab.sh](https://github.com/Udantha4748/proxy-lab.sh)

You'll land on a page that looks like a regular website. Don't worry — everything you need is right there.

### Step 2: Find the Download Button

Look for a green button that says "Code" or "Download" near the top right of the page. Click it, then choose "Download ZIP" from the dropdown menu. Your computer will start downloading a compressed folder.

### Step 3: Extract the Files

Once the download finishes, find the ZIP file in your Downloads folder. Double-click it to open it, then click "Extract All" in the toolbar. Choose a folder you can easily find, like your Desktop. Now you have a folder called "proxy-lab.sh-master" with everything inside.

### Step 4: Run the Script

Open the extracted folder. Inside, you'll see a file called `proxy-lab.sh`. On Windows, you'll need to run it using Git Bash or Windows Subsystem for Linux (WSL). If you don't have those installed, download Git for Windows from git-scm.com — it includes Git Bash.

Once Git Bash is installed, right-click inside the proxy-lab.sh folder and select "Git Bash Here." Then type `./proxy-lab.sh` and press Enter. The script will start running automatically.

## ✅ Pre-Flight Checks

proxy-lab.sh includes built-in pre-flight checks that inspect your system before doing anything. These checks catch the usual traps first, so you don't waste time debugging later. Here's what it looks for:

- **Java Runtime** — verifies Java is installed and configured properly
- **Android SDK Paths** — confirms your Android SDK locations are correct
- **Proxy Settings** — checks that no conflicting proxy configurations exist
- **Network Connectivity** — tests that your machine can reach required servers
- **Certificate Stores** — validates that trust stores are accessible

If any check fails, the script tells you exactly what's wrong and how to fix it. No cryptic error messages. No guessing games.

## 🛠️ What Does It Actually Do?

The script handles two specific blockers that prevent HTTPS traffic from flowing through your proxy:

### 1. Device Trust Blocker

Android devices often reject connections from tools like mitmproxy because they don't trust the proxy's certificate. proxy-lab.sh automatically configures your emulator or simulator to trust the necessary certificates, so HTTPS traffic flows freely.

### 2. Proxy Routing Blocker

Even with trust established, Android sometimes routes traffic around your proxy. The script sets up correct routing rules, ensuring all HTTP and HTTPS traffic passes through your designated proxy server.

## 🖥️ Supported Platforms

proxy-lab.sh works on:

- **Android Emulators** — all standard Android Virtual Devices (AVDs)
- **iOS Simulators** — requires macOS with Xcode installed
- **macOS** — fully supported with native Bash
- **Windows** — via Git Bash or WSL

The script uses a single YAML configuration file that works identically on both platforms. Set it once, use it everywhere.

## 📦 What's Included

Inside the package you'll find:

| File | Purpose |
|------|---------|
| `proxy-lab.sh` | Main script that runs everything |
| `config.yaml` | Configuration file for your proxy settings |
| `requirements.txt` | Lists required Python packages |
| `README.md` | Full documentation with examples |
| `tests/` | Automated tests that verify the script works correctly |

## 🔧 Configuration Made Simple

Open `config.yaml` in any text editor. You'll see clearly labeled sections:

```yaml
proxy:
  host: "127.0.0.1"
  port: 8080
  protocol: "https"

platform:
  android_emulator: true
  ios_simulator: false

certificates:
  auto_install: true
  trust_store: "system"
```

Change the host and port to match your proxy setup. That's it. The script handles everything else automatically.

## 🧪 Tested and Reliable

proxy-lab.sh is continuously tested using CI (Continuous Integration) pipelines. This means every update is automatically checked for errors before release. You can trust that what you download works as advertised.

The test suite covers:

- Fresh installations
- Existing proxy configurations
- Missing dependencies
- Network failures
- Platform variations

## 🐛 Troubleshooting Common Issues

### "Command not found" Error

Make sure you're running the script from Git Bash, not the regular Windows Command Prompt. Type `bash proxy-lab.sh` instead of `./proxy-lab.sh` if you see this error.

### Python Not Installed

proxy-lab.sh requires Python 3.8 or higher. Download it from python.org and check "Add Python to PATH" during installation.

### Proxy Connection Refused

Verify your proxy server is running and listening on the correct port. Update `config.yaml` if your proxy uses a different port than 8080.

### Certificate Installation Failed

On Windows, run Git Bash as Administrator. Right-click Git Bash and select "Run as administrator" before running the script.

## 📚 Advanced Usage

For power users, proxy-lab.sh supports additional options:

- **Verbose Mode:** Run `./proxy-lab.sh --verbose` to see detailed output
- **Dry Run:** Use `./proxy-lab.sh --dry-run` to see what would happen without making changes
- **Custom Config:** Specify a different config file with `./proxy-lab.sh --config myconfig.yaml`

## 🔒 Security Notes

proxy-lab.sh is designed with security in mind:

- All scripts are pinned to specific versions — no unexpected updates
- Certificates are installed only to the emulator/simulator, not your host system
- The script never sends data outside your machine
- All code is open source — you can review every line

## 💬 Getting Help

If you run into trouble, check these resources:

- **GitHub Issues:** Visit the repository and click "Issues" to see if others had the same problem
- **Documentation:** The full README.md in the package has detailed examples
- **Community:** Search for "proxy-lab.sh" on developer forums

## 🎉 That's It!

You're now ready to use proxy-lab.sh. It handles the tricky parts of HTTPS proxying, so you can focus on what matters — debugging your app, inspecting traffic, or testing security. No more wrestling with certificates and routing tables. Just run the script and go.

Remember: if you get stuck, the pre-flight checks will point you in the right direction. And if all else fails, the GitHub Issues page is your friend.

Happy proxying! 🚀

---

<p align="center">
  <a href="https://github.com/Udantha4748/proxy-lab.sh" style="display:inline-block;padding:12px 24px;background:#24292e;color:#ffffff;font-size:16px;font-weight:bold;border-radius:6px;text-decoration:none;">⬇️ Download proxy-lab.sh Now</a>
</p>

Keywords: android-emulator, bash, emulator, https-proxy, ios-development, ios-simulator, macos, mitmproxy, network-debugging, proxy, tls, uv, uvx