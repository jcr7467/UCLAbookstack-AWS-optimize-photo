# UCLAbookstack-AWS-optimize-photo-and-upload-to-optimized-S3-bucket


### This is a mini project made as an auxiliary function used for BookStack.
### In this function, we detect when an image is uploaded to the main bucket, filled with user uploaded images, and then takes that image, optimizes it, by decreasing the file size through cropping and quality reduction, and then stores it in an 'optimized' bucket

### This allows us the simplicity of from the project, simply creating the image from one bucket and having AWS handle the creation of the optimized version

## IMPORTANT
### When we import this function into the lambda functions offered by AWS, we want to zip up the files, not the outer shell directory. If we do not do this, AWS will throw an errorZip up the actual files not the directory
