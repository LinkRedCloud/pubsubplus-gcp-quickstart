# solace-gcp-quickstart

## Create a base image
1. Create and instance based off of Centos 7 with 2 CPU and 6GB memory, and 30GB disk space.
2. Cut and past the contents of pre-install into the google web shell.
3. Ensure the instance does not delete disk on delete.
4. Delete the instance.
5. Promote the disk to a custom image.
   https://console.cloud.google.com/compute/imagesAdd?_ga=1.189267755.1234043161.1488336718
   set Name<solace-base-iname> Family<solace> Description<Solace base image> Source<disk> Source Disk<Yourdisk>

## Use the custom image
1. Create and instance based off of custom image with 2 CPU and 6GB memory, and 30GB disk space.
2. Set security rules allow desired protocol access