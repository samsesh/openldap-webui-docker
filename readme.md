# OpenLDAP & WebUI on Docker🐳 🚀

Welcome to the **OpenLDAP & WebUI on Docker🐳** project! This repository provides a Docker setup for running OpenLDAP with a web-based user interface, making it easier to manage and interact with your LDAP server.

## 📦 Features

- Easy Docker setup for OpenLDAP with WebUI.
- Web-based interface for LDAP management.
- Configurable and extensible Docker setup.

## 🛠️ Getting Started

### Prerequisites

- Docker: Ensure you have Docker installed on your machine. You can get it from [Docker's official site](https://www.docker.com/get-started).

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/samsesh/openldap-webui-docker.git
   cd openldap-webui-docker
   ```

2. **Prepare Configuration:**

   Copy the example environment file to `.env`:

   ```bash
   cp env-exam .env
   ```

   Open the `.env` file and adjust the configuration variables as needed. This includes setting the LDAP admin password and other environment-specific settings.

3. **Build and Run the Docker Containers:**

   ```bash
   docker-compose up -d
   ```

   This command will build the Docker images (if needed) and start the OpenLDAP and WebUI services in detached mode.

4. **Access the WebUI:**

   Open your web browser and navigate to `http://localhost:8080` to access the OpenLDAP WebUI.

### 🔑 How to Login

1. **Open the WebUI:**

   Go to `http://localhost:8080` in your web browser.

2. **Login Credentials:**

   - **Username:** `cn=admin,dc=example,dc=com`
   - **Password:** `admin`

   These credentials are set in the `.env` file by default. If you changed them, use the updated credentials.

## 🔧 Configuration

The Docker setup uses `docker-compose.yml` and `.env` for configuration. You can adjust settings such as ports, volumes, and environment variables in these files.

## 📚 Documentation

For more details on how to use OpenLDAP and its WebUI, refer to the official [OpenLDAP documentation](https://www.openldap.org/doc/admin24/).

## 🚀 Contributing

We welcome contributions to improve this project! If you have suggestions or issues, please [open an issue](https://github.com/samsesh/openldap-webui-docker/issues) or submit a pull request.

## 💖 Donate

If you appreciate this project and would like to support its development, please consider donating. You can find more information and donate [here](https://github.com/samsesh/donate).

---

Happy LDAP management! 🧑‍💻🎉