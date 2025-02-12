You can install Git on macOS by following these steps:

---

### **1. Check if Git is Already Installed**
Open the **Terminal** (`Cmd + Space`, type **Terminal**, and press **Enter**) and run:

```sh
git --version
```

If Git is installed, it will display the installed version. If not, follow the steps below.

---

### **2. Install Git Using Homebrew (Recommended)**
#### **Step 1: Install Homebrew (If Not Installed)**
Homebrew is a package manager for macOS. If you don’t have it, install it by running:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

After installation, update Homebrew:

```sh
brew update
```

#### **Step 2: Install Git**
Once Homebrew is installed, run:

```sh
brew install git
```

#### **Step 3: Verify Installation**
After installation, check the Git version:

```sh
git --version
```

If installed correctly, it will show the version number.

---

### **3. Alternative: Install Git via Xcode Command Line Tools**
If you prefer not to use Homebrew, you can install Git using Apple’s Xcode command-line tools:

```sh
xcode-select --install
```

A pop-up will appear—click **Install** and wait for the process to complete.

Once installed, verify using:

```sh
git --version
```

---

### **4. (Optional) Configure Git**
Set up your Git username and email:

```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

Now, Git is installed and ready to use on your Mac! 🚀
