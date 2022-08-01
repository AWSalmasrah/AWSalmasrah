# Host a static website on S3

- Create S3 bucket
    - Uncheck "Block all public access"
    - Properties > Static website hosting (get the URL of the bucket).
    - Permisions > Bucket Policy > 

```
    {
      "Version":"2012-10-17",
      "Statement":{
          "Effect":"Allow",
          "Principal": "*",
          "Action":"s3:GetObject",
          "Resource":"ARN/*"
      }
    }
```
