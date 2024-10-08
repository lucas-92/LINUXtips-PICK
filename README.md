## Practical Project Challenge - PICK 2024_01

**Objective:** Implement and configure the application with the listed technologies, ensuring high standards of security, automation and monitoring.

#### Project Requirements:

1. [**Containerization with Docker:**](https://github.com/lucas-92/LINUXtips-PICK/blob/main/docs/1.%20Containerization%20with%20Docker.md) 
   - Containerize the password management application.
   - Create an efficient and secure `Dockerfile`.
   - Publish the Docker image to a public repository.

2. [**Orchestration with Kubernetes:**](https://github.com/lucas-92/LINUXtips-PICK/blob/main/docs/2.%20Orchestration%20with%20Kubernetes.md)
   - Deploy the application on Kubernetes.
   - Create the necessary manifests (`Deployment`, `Service`, `ConfigMap`, `Secret`, etc.).
   - Use `Ingress` to expose the application externally.

3. [**Deploy Automation with Helm:**](https://github.com/lucas-92/LINUXtips-PICK/blob/main/docs/3.%20Deploy%20Automation%20with%20Helm.md)
   - Create a Chart Helm for the application.
   - Configure dynamic values ​​for different environments (dev, staging, prod).
   - Generate Helm packages and store in a public Helm repository.

4. [**Security Policies with Kyverno:**](https://github.com/lucas-92/LINUXtips-PICK/blob/main/docs/4.%20Security%20Policies%20with%20Kyverno.md)
   - Create Kyverno policies to ensure security practices such as:
     - Verification of signed images.
     - Prohibition of running as root.
     - Checking sensitive environment variables.
   - Implement compliance policies.

5. **Image Signature with Cosign:**
   - Sign Docker images using Cosign.
   - Configure automatic signature verification in Kubernetes using Kyverno policies.

6. [**Monitoring with Prometheus:**](https://github.com/lucas-92/LINUXtips-PICK/blob/main/docs/6.%20Monitoring%20with%20Prometheus.md)
   - Implement customized metrics in the application.
   - Configure Prometheus to collect and visualize these metrics.
   - Create alerts based on application-specific metrics.

7. [**Package Distribution with APKO and Melange:**](https://github.com/lucas-92/LINUXtips-PICK/blob/main/docs/7.%20Package%20Distribution%20with%20APKO%20and%20Melange.md)
   - Use Melange to create application packages.
   - Configure a CI/CD pipeline to build and distribute these packages.
   - Ensure packages are available for different environments (dev, staging, prod)
