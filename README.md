# AWS S3 file upload progress (aws-upload-s3)
AWS S3 file upload with progress bar 

## Feature 
1. File Upload 
2. Progress bar

<strong>Note:</strong> ap-southeast-1 is the default AWS region setting.

## Enable CORS
Make sure your AWS S3 CORS settings for your bucket look something like this:
```json
[
    {
        "AllowedHeaders": [
            "*"
        ],
        "AllowedMethods": [
            "PUT",
            "POST",
	    "GET",
	    "HEAD",
            "DELETE"
        ],
        "AllowedOrigins": [
            "*"
        ],
        "ExposeHeaders": [
            "ETag"
        ]
    }
]
```

## Enable ACLs
Go to your bucket, into the Permissions tab, find Object Ownership and click Edit. Select ACLs enabled and read carefully AWS warnings about potential security risks

## Allow public access
Set Block new public ACLs and uploading public objects to false

## Usage
index.html
HTML upload form

style.css
Style for progress bar

app.js
```javascript
accessKeyId: "ACCESS_KEY", //update your access key
secretAccessKey: "SECRET_KEY", //update your secret key
Bucket: "BUCKET_NAME", //update your bucket name
folderName = "Document/"; //update your prefix path
uniqueFileName = 'SampleFile.mp4';  //update your file name
```
   
## Reference : 
https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/s3-example-photo-album.html
