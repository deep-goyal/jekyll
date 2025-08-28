---
title: System Setup
layout: home
---

# **System Setup**
{: .no_toc}
---



Welcome to CSE355\! The first half of this course covers Finite and Pushdown Automata. To help you design and test your machines, the instructional team has developed `cse355-machine-design`, a Python package that lets you instantly test your designs against various input strings.

To ensure a clean and conflict-free setup, we'll use a **virtual environment** (`venv`). This is a standard practice that creates an isolated space for this course's packages, so they don't interfere with other Python projects on your machine.

- TOC
{:toc}

### **Step 0: Check Your Python Version (All Platforms)**

Before you begin, open your terminal (Terminal on Mac/Linux, PowerShell or CMD on Windows) and check your Python version. We require **Python 3.10 or newer**.

```bash
# On macOS and Linux
python3 --version

# On Windows
py --version
```

If you don't have Python or have an older version, please install the latest stable version from [python.org](https://www.python.org/downloads/).

### **Step 1: Create Your Project Directory**

Before creating the environment, create a dedicated folder for your coursework and navigate into it.

```bash
mkdir cse355-projects
cd cse355-projects
```

-----

## **Macintosh**

Modern macOS versions come with Python 3. If the `python3 --version` command failed, you may need to install the [Xcode Command Line Tools](https://developer.apple.com/xcode/resources/) by running `xcode-select --install`.

1.  **Create the virtual environment** in your project folder:

    ```bash
    python3 -m venv venv
    ```

2.  **Activate the environment.** This command tells your terminal to use the Python and tools inside the `venv` folder.

    ```bash
    source venv/bin/activate
    ```

    You'll know it worked when you see `(venv)` at the beginning of your terminal prompt.

3.  **Upgrade `pip` and install the package:**

    ```bash
    pip install --upgrade pip
    pip install cse355-machine-design
    ```

4.  **When you're done,** exit the environment with:

    ```bash
    deactivate
    ```

-----

## **Linux** 

This section assumes you are using a Debian-based distro (like Ubuntu) with the `apt` package manager. For other distros, use your native package manager (e.g., `dnf` for Fedora, `pacman` for Arch).

1.  **Install python, pip, and venv.** These are often in separate packages.

    ```bash
    sudo apt update
    sudo apt install python3 python3-pip python3-venv
    ```

2.  **Create the virtual environment** in your project folder:

    ```bash
    python3 -m venv venv
    ```

3.  **Activate the environment:**

    ```bash
    source venv/bin/activate
    ```

    Your terminal prompt should now start with `(venv)`.

4.  **Upgrade `pip` and install the package:**

    ```bash
    pip install --upgrade pip
    pip install cse355-machine-design
    ```

5.  **To exit the environment,** simply run:

    ```bash
    deactivate
    ```

-----

## **Windows** 

1.  **Download and install Python** from the [official website](https://www.python.org/downloads/windows/).

      - **CRITICAL:** On the first screen of the installer, you **must** check the box that says **"Add Python to PATH"**. This will save you a lot of trouble.

2.  **Create the virtual environment** in your project folder:

    ```bash
    py -3 -m venv venv
    ```

3.  **Activate the environment.** The command is different depending on whether you are using Command Prompt or PowerShell.

      - **For PowerShell:**

        ```powershell
        .\venv\Scripts\Activate.ps1
        ```

        *(If you get an error about execution policies, run `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process` and try again.)*

      - **For Command Prompt (CMD):**

        ```cmd
        venv\Scripts\activate
        ```

    You will see `(venv)` at the start of your prompt once it's active.

4.  **Upgrade `pip` and install the package:**

    ```bash
    pip install --upgrade pip
    pip install cse355-machine-design
    ```

5.  **When you're finished,** use this command to leave the environment:

    ```bash
    deactivate
    ```