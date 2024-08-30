# Overview
This repository serves as a template for setting up a comprehensive Java development environment in GitHub Codespaces, specifically tailored for projects that require a graphical user interface (GUI). Traditionally, running GUI applications within a GitHub Codespace poses significant challenges due to the limitations of headless environments. However, this template overcomes these limitations by integrating a NoVNC viewer, allowing developers to run and interact with GUI applications directly within their Codespace.

By leveraging NoVNC, this template makes it possible to display the Java GUI in a separate browser tab, providing a seamless development experience as if you were working on a local machine. This is particularly useful for developers building desktop applications, educational tools, or any other Java-based project that requires a visual interface.

# Key Features
- **Java 21 Environment:** The template is configured to use Java 21, ensuring compatibility with the latest Java features and improvements.
- **Gradle Build System:** The project uses Gradle as its build system, making it easy to manage dependencies, build the project, and run tests.
- **Pre-configured Dev Container:** The repository includes a `.devcontainer` directory with configuration files that define the development environment, including a `Dockerfile` and a `devcontainer.json` file.
- **VNC and NoVNC Integration:** The environment supports running graphical applications within the Codespace via VNC, accessible through a web browser using NoVNC.
- **Automated Setup Script:** The repository includes a `run_with_xvfb.sh` script that automates the setup of Xvfb, x11vnc, and the Openbox window manager, ensuring the graphical environment is ready to use upon startup.
- **Customizable Ports:** The configuration forwards essential ports (5900 for VNC and 6080 for NoVNC), making it easy to connect to the graphical environment from different devices.

# Usage
To start using this template, simply clone the repository and open it in GitHub Codespaces. The environment will be automatically set up according to the configuration files. You can start coding immediately, using the latest Java tools and technologies.

# Update the Following Files

Ensure to update the following files as necessary:

- `/workspaces/codespaces-blank/.devcontainer/run_with_xvfb.sh` - Line 36
- `/workspaces/codespaces-blank/build.gradle` - Line 32
- `/workspaces/codespaces-blank/settings.gradle` - Line 14
