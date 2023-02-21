## Challenge 3

Create two Jenkins pipelines for deploying both images from Challenge 1 and Challenge 2 to a specified environment (e.g. dev, staging, production). The pipelines should ensure that:

- The latest version of the images are built and pushed to a Docker registry
- Secrets are securely managed and not committed to the repository
- The appropriate environment variables are set
- The images are deployed to a specified environment and the appropriate ports are exposed

Please note that in addition to Jenkins, you will also need access to a Docker registry, such as Docker Hub or a private registry, to push the images.

Please submit your solution in the form of a pipeline script.
