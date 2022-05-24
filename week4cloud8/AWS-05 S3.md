# [Simple Storage Service]

Learn about S3 services, storage classes, Glacier deep Archive, Pricing, 

Build buckets, fill them with data, give acces and share with other peers

## Key terminology

There are 4 storage classes:
S3 Standard
S3 Standard-IA
S3 One-zone IA
S3 Glacier
There’s also S3 Glacier Deep archive, a subclass of S3 Glacier. And Intelligent Tiering which is more a cost optimization tool than a class on its own.
Storage classes differ in availability, durability, retrieval time, and cost.

## Exercise
Exercise 1
Create new S3 bucket with the following requirements:
Region: Frankfurt (eu-central-1)
Upload a cat picture to your bucket.
Share the object URL of your cat picture with a peer. Make sure they are able to see the picture.

Exercise 2
Create new bucket with the following requirements:
Region: Frankfurt (eu-central-1)
Upload the four files that make up AWS’ demo website.
Enable static website hosting.
Share the bucket website endpoint with a peer. Make sure they are able to see the website.


### Sources
[AWS console solutions](https://eu-central-1.console.aws.amazon.com/console/home?region=eu-central-1#)

### Overcome challanges
Finding the solution to share expercise 2 website,  make it accesable
### Results

**Exercise 1**

Result:
![catpic](../00_includes/catpic.png)

**Exercise 2**
 
Result: 
![s3website](../00_includes/Websites3.png)
