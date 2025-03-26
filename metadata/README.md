In this folder I am setting metatags on an S3 file. The following are the steps.

#### Create a bucket

aws s3 mb s3://metadata-understanding-evan

### Create a new file

echo "Hello Jupiter" > hello.txt

### Upload file with MetaData

aws s3api put-object --bucket metadata-understanding-evan --key hello.txt --body hello.txt --metadata Planet=Jupiter 

### Getting Metadata through HeadObject

aws s3api head-object --bucket metadata-understanding-evan --key hello.txt


#### Outout from head

aws s3api head-object --bucket metadata-understanding-evan --key hello.txt
{
    "AcceptRanges": "bytes",
    "LastModified": "2025-03-26T17:17:16+00:00",
    "ContentLength": 14,
    "ETag": "\"6376188c6ad3f0b3dc754e4ca2b0d122\"",
    "ContentType": "binary/octet-stream",
    "ServerSideEncryption": "AES256",
    "Metadata": {
        "planet": "Jupiter"
    }
}

####Clean up

aws 