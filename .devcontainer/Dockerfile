# Start with a base image that has the necessary tools you need
# For example, you can use an image that already has Node.js, Python, or any other dependencies you require.
# Replace "base-image" with the appropriate base image.
FROM base-image:latest

# Install additional dependencies if needed
# For example, if you need to install specific packages or tools, use the package manager of your base image.
RUN apt-get update && apt-get install -y \
    package-1 \
    package-2 \
    package-3

# Set the working directory inside the container
WORKDIR /home/src

# (Optional) If you want to copy additional files into the container, you can use the COPY command.
# For example, if you have additional scripts or configuration files, you can copy them to the container.
# COPY my-script.sh /home/src/

# (Optional) Set any environment variables if required.
# ENV MY_ENV_VAR=value

# (Optional) Run any additional setup commands inside the container
# For example, you may need to run a setup script specific to your project.
# RUN ./setup.sh

# (Optional) If you need to forward specific ports from the container to the Codespace, you can use the EXPOSE command.
# For example, if your application runs on port 6789 inside the container and you want to access it from the Codespace.
EXPOSE 6789

# (Optional) You can specify the default command to run when the container starts.
# For example, if you want to start your application automatically using the 'mage' command.
CMD ["mage", "start", "demo_project"]
