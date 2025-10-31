# Liferay Setup with DDEV

A simple and fast setup to run **Liferay Portal** locally using **DDEV**, a powerful environment for web development.

---

## 🚀 Prerequisites

Ensure you have the following tools installed on your system before starting:

* **1. DDEV:** The primary tool for managing the local environment.
* **2. Docker:** Used by DDEV to run containers.
* **3. Git:** To clone this repository.

---

## 🛠️ Installation Steps

Follow these steps in your terminal to get Liferay up and running:

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/sharaddevops83/liferay-setup.git
    ```

2.  **Navigate to the Project Directory**
    ```bash
    cd liferay-setup
    ```

3.  **Configure DDEV**
    This sets up DDEV for a PHP project with the `web` folder as the document root.
    ```bash
    ddev config --project-type=php --docroot=web --create-docroot
    ```

4.  **Start the Environment**
    ```bash
    ddev start
    ```

5.  **Access the Container Shell**
    ```bash
    ddev exec bash
    ```

6.  **Move to the Web Root**
    ```bash
    cd /var/www/html
    ```

7.  **Run the Liferay Setup Script**
    This script handles the download and initial setup of Liferay Portal within the container.
    ```bash
    bash setup-liferay.sh
    ```

8.  **Access Liferay in Browser**
    Open your web browser and go to the project's URL:
    * **http://liferay-setup.ddev.site:8080**

9.  **Complete Setup**
    Follow the Liferay setup wizard prompts to finalize the installation.

---

## 🔑 Default Credentials

After the initial setup is complete, you can log in using these default credentials:

| Role | Username | Password |
| :--- | :--- | :--- |
| **Admin** | `test@liferay.com` | `test` |
