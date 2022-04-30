# Create a new gitlab repo group for the product that will hold all repos. In our case we created a group called project-x

# Add your registry credentials as CI/CD variables for the full group. We have created REG_PASSWORD and REG_USER which is used in the gitlab pipeline to login to Docker Hub to push and pull the images 