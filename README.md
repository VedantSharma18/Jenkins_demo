# Jenkins Installation and Setup Guide

## Download Jenkins

1. Go to the Jenkins download page: [Jenkins Download](https://www.jenkins.io/download/#downloading-jenkins)

## Installation Steps

- **Windows:** Follow the steps provided here: [Windows Installation](https://www.jenkins.io/doc/book/installing/windows/#windows-msi-installers)
- **macOS:** Follow the steps provided here: [macOS Installation](https://www.jenkins.io/download/lts/macos/#homebrew-installer)

## Troubleshooting

- **Windows:** Refer to the troubleshooting guide: [Troubleshooting Windows Installation](https://www.jenkins.io/doc/book/installing/windows/#troubleshooting-windows-installation). To open Administrative Tools, go to Control Panel and paste the following path in the address bar:
    ```
    Control Panel\System and Security\Windows Tools
    ```

## Initial Setup and Plugin Installation

1. After installing Jenkins, open your web browser and go to `http://localhost:8080`.
2. Follow the instructions to unlock Jenkins using the initial admin password.
3. Install the suggested plugins when prompted.

## Managing Jenkins Service

Jenkins runs on port 8080 by default. If you need to stop Jenkins:

- **Windows:**
  1. Go to Start and search for "Services".
  2. In the Services window, search for "Jenkins".
  3. To stop the service, right-click on "Jenkins" and select "Stop".
  4. To start the service again, right-click on "Jenkins" and select "Start".

- **macOS:**
  - Stop Jenkins service: 
    ```sh
    brew services stop jenkins-lts
    ```
  - Start Jenkins service:
    ```sh
    brew services start jenkins-lts
    ```

---