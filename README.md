# Hosting-a-static-website
## Hosting a static website with S3
Simple Storage Service is an AWS storage service used to store unlimited amounts of data. It is bound to a specific region. Data are stored as Objects in Buckets. S3 can be used to host content for static websites. I used the Standard tier which is highly available as it automatically updates your data in three Availability Zones.  
### Steps
Sign in to the AWS Management Consoles and open the S3 console.
 
Click on Buckets on the Navigation Pane, and Create Bucket.

Type in a globally unique name. It cannot contain uppercase and must be between 3 and 63 characters long.

Next, choose the AWS Region where you want your data to be stored.

Under Object Ownership, disable the Access Control list if only you want to have full control and access over your Bucket.

Block Public Access Should be disabled since we are hosting a website that we want the public to access.

Next, copy the source code of the website and upload it into the Bucket.

Go to Bucket properties and enable static website hosting, type the name of the index document, and save changes.

Now to give the public access to the website click on permissions then Bucket policy and paste the Bucket policy to give all Users access to your Bucket. Edit the name of the Bucket in the Policy to your Bucket name

Go back to your bucket and copy the URL of the index.html to access your websites

<img width="960" alt="website final" src="https://user-images.githubusercontent.com/110430121/192836851-4279695a-abd6-4224-b91b-a68db633e65b.png">

