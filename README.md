# AWS S3 file upload progress (aws-upload-s3)
AWS S3 file upload with progress bar 

## Feature 
1. File Upload 
2. Progress bar

<strong>Note:</strong> us-east-1 is the default AWS region setting.

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

## Usage


## Reference : 
https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/s3-example-photo-album.html
