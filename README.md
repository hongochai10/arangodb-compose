# Introduction
This project uses Docker Compose to deploy ArangoDB, a powerful NoSQL database. The `compose.yaml` file defines the configuration for the ArangoDB service, including parameters such as version, resources, environment variables, and networks.

# Directory Structure
- `compose.yaml`: Configuration file for Docker Compose.
- `.env`: File containing the necessary environment variables for configuring the service.
- `.gitignore`: File to specify files that are not needed for version control.

# How to Use
1. **Install Docker and Docker Compose**: Ensure that you have Docker and Docker Compose installed on your machine.
2. **Create Docker Network**: Before starting the service, you need to create the `baota_net` network using the following command:
   ```bash
   docker network create baota_net
   ```
3. **Configure Environment Variables**: Open the `.env` file and adjust variables such as `VERSION`, `HOST_IP`, `PORT`, and `PASSWORD` according to your needs.
4. **Start the Service**: Run the following command in the directory containing the `compose.yaml` file:
   ```bash
   docker-compose up -d
   ```
5. **Access ArangoDB**: After the service starts, you can access ArangoDB through your browser at the address `http://<HOST_IP>:<PORT>`.

# Note
- Ensure that you have created the `baota_net` network before starting the service.
- Check your system resources to ensure that it can meet the limits specified in the `compose.yaml` file.

# Contact
If you encounter any issues, please contact the author Ho Ngoc Hai or open an issue in the project's GitHub repository.

# License
This project is licensed under the MIT License. You are free to use, copy, modify, and distribute the source code, as long as you include the copyright notice and license in all copies or substantial portions of the software.

# Thank you for using ArangoDB!
