---
title: System Setup
layout: home
---

# **System Setup**
{: .no_toc}

The first half of CSE355 covers Finite Automatas and Pushdown Automatas.
[Saajan Maslanka](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://www.linkedin.com/in/saajanm&ved=2ahUKEwjYhNf38KuPAxVXJkQIHUv3PDwQFnoECBsQAQ&usg=AOvVaw331PylTzK2S4H8hCbhGZIJ) along with the CSE355 instructional team have developed [cse355-machine-design](https://pypi.org/project/cse355-machine-design/), a python package to help you input your FAs and PDAs and test it
against a variety of strings instantly.

- TOC
{:toc}

## Macintosh

The Macintosh OS ships with python pre-installed. You can follow these steps to initialize a virtual environment and install the package into the environment.

- Create a virtual environment by running:

  ```bash
  python3 -m venv venv
  ```

- Use this virtual environment with:

  ```bash
  source ./venv/bin/activate
  ```

- Load the package into the environment by downloading it from pip with:

  ```bash
  pip install cse355-machine-design
  ```

## Linux

This section assumes you are using `apt` package manager in your distro.

- Download python:

  ```bash
  apt-get install python
  ```


- Create a virtual environment by running:

  ```bash
  python3 -m venv venv
  ```

- Use this virtual environment with:

  ```bash
  source ./venv/bin/activate
  ```

- Load the package into the environment by downloading it from pip with:

  ```bash
  pip install cse355-machine-design
  ```

## Windows

- Download [Python Installer](https://www.python.org/downloads/windows/) for Windows

- After configuring python for your machine, initialize a virtual environment by running:

  ```bash
  python3 -m venv venv
  ```

- Load the virtual environment and install the package by running these commands in powershell:

  ```sh
  .\venv\Scripts\Activate.ps1
  pip install cse355-machine-design
  ```
