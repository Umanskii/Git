You can install Git on Windows by following these steps:

### **1. Download Git for Windows**
- Visit the official Git website: [https://git-scm.com/download/win](https://git-scm.com/download/win)
- The download should start automatically. If not, click on the provided link for the latest version.

### **2. Run the Installer**
- Locate the downloaded `.exe` file (usually in the **Downloads** folder) and double-click it to start the installation.

### **3. Configure Installation Settings**
- **Select Destination Location**: Choose where to install Git (default: `C:\Program Files\Git\`).
- **Select Components**: Keep the default selection unless you need additional features.
- **Adjust PATH Environment**: Choose **"Git from the command line and also from 3rd-party software"** (recommended).
- **Select HTTPS Library**: Use the default **OpenSSL**.
- **Choose Line Ending Conversion**: 
  - **Windows-style (CRLF)** if working mainly with Windows.
  - **Unix-style (LF)** if collaborating with Linux/macOS users.
- **Choose Terminal Emulator**: Default is **MinTTY** (recommended). You can also select the **Windows Command Prompt** if needed.
- **Configure Default Git Editor**: Choose an editor like **Vim** (default) or **VS Code**, **Notepad++**, etc.
- Keep the remaining options as default and click **Install**.

### **4. Verify Installation**
After installation, open **Command Prompt** or **Git Bash** and type:

```sh
git --version
```

If installed correctly, it will display the installed Git version.

### **5. (Optional) Configure Git**
Set up your name and email:

```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Now, Git is ready to use on Windows! 🚀
