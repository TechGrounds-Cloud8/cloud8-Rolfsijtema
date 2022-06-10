What is CDN?

- A worldwide Content Delivery Network that distributes a group of servers that work together.

- It caches content to servers closer to your physical location, this will provide a faster delivery of content. 

- The Main server (Origin) sends a copy of the content, that is asked frequently.  to a  edgelocation-server. 

-  When data is les populair it delete’s the content from the edge-location.

What is Cloudfront:

- There are many Content Delivery Network’s but today we speak about AWS Cloudfront.

- Amazon Cloudfront is a webservice that speeds up distribution of your static and dynamic web content, Could be: HTML, Images or video content  to for example end-users. 

- Cloudfront automatically delivers your content to the worldwide network of Data-centers called Edge-locations.  

- Cloudfront Increases reliability and Availability

- Lower Latency because the end-users are closer to the Edge-server-locations compare to the Origin-server. 


- Global Edge Network

	- On the slide you find an example of Edge-locations that are located around the world.  

- These are the locations where copy’s of populair content are send to from the Origen-server. 

- This network is constantly growing, more than 300 at the moment.

-  country’s or states can have more than 1 edge-location. 


Cloudfront & S3

- A match made in the Cloud, Why?

- The S3 bucket is the place you already have ur data content, CloudFront makes the use of these buckets / content a lot quicker. 

- Auto scaling, scalability.

- More efficiency in cost and Energy

- Uses the already configured secure-data in S3 buckets

Summary: 

* CDN is a globally distributed set of servers that caches content
* 
* Makes everything quicker! 
* 	
* CloudFront is a AWS-CDN using Edge Locations
* 
* It is growing constantly
* 
* S3 is very compatible with Cloudfront



Questions;




What do you pay for in S3?
* GB storage per month
* Transfer OUT to out of the region
You don’t pay for:
* Transfer IN to Amazon S3
* Transfer OUT from S3 to CloudFront or EC2 in the same region


