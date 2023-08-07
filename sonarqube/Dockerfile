# Use the official SonarQube image
FROM sonarqube:latest

# Switch to the root user for installing packages
USER root

# Install Vim
RUN apt-get update && \
    apt-get install -y vim && \
    rm -rf /var/lib/apt/lists/*

# Switch back to the non-root SonarQube user
USER sonarqube

# Expose the SonarQube port (adjust if necessary)
EXPOSE 9000
