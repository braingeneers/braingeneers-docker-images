# Braingeneers Docker Images

Welcome to the Braingeneers Docker Image repository! This repository is dedicated to providing users with Docker images tailored for building GitHub Codespaces with the necessary infrastructure for classroom and research purposes. The images are built daily using GitHub Actions to ensure you have access to the latest updates and features.

## Repository Contents

### Docker Images

The repository contains two main Docker images:

1. **Classroom Image:** This image provides the basic infrastructure required for educational purposes.

2. **Research Image:** This image is designed for research activities and includes additional tools and libraries.

### Key Files

Inside the Docker images, you'll find the following key files:

- **Dockerfile:** The Dockerfile serves as the blueprint for creating the images. It is based on the PANGEO base image and includes all the necessary configurations and dependencies.

- **apt.txt:** This file allows users to specify additional bash or shell packages they want to install within the Docker image. You can customize this file according to your requirements.

- **environment.yml:** The environment.yml file allows users to define the libraries and packages they want to install using Conda Forge. This is particularly useful for setting up specific Python environments.

- **postBuild:** The postBuild script is executed during the image build process. It automatically installs the latest `braingeneerspy` library and datasets into the `/home/joyvan/data/*` directory, ensuring you have access to the latest data and tools.

## Usage

To use these Docker images, follow these steps:

1. **Pull the Image:** You can pull the latest version of the desired image from the GitHub Container Registry (GHCR) [classroom image](https://github.com/Braingeneers/braingeneers-docker-images/pkgs/container/classroom) or [research image](https://github.com/Braingeneers/braingeneers-docker-images/pkgs/container/research) by running:

   ```bash
   docker pull ghcr.io/braingeneers/classroom:latest
   ```

   or

   ```bash
   docker pull ghcr.io/braingeneers/research:latest
   ```

2. **Customize as Needed:** If you have specific requirements, you can customize the Docker image by modifying the `apt.txt` and `environment.yml` files. This allows you to install additional packages and libraries as required.

3. **Build a Codespace:** You can use these Docker images to create GitHub Codespaces for your classroom or research projects. Refer to the GitHub Codespaces documentation for instructions on how to set up a Codespace using a custom Docker image.

## Contribution

Contributions to this repository are welcome! If you have improvements, additional features, or bug fixes to suggest, please submit a pull request. Your contributions will help enhance the usability and functionality of these Docker images for the Braingeneers community.

Thank you for using Braingeneers Docker Images for your educational and research endeavors!

[Visit Braingeneers Website](https://braingeneers.ucsc.edu)
