
# Udacity Static Website Hosting Project

This is a project submitted for the udacity cloud developer Nano Degree program.



## Steps For hosting this static website using AWS S3 Bucket to Cloudfront Distribution



### step 1: Create S3 bucket


![This is an image](https://raw.githubusercontent.com/sewunet/Udacity-Project-1/master/Screenshot/create%20Bucket.PNG)



### Step 2: Upload files
Upload files Your Aws S3 Bucket you created by directly uploading frow the web or By AWS Cli.
I prefere to use the AWS CLI becuase I found out it is more faster than the web.

**Verify the AWS CLI configuration. If not configured already, use:**
```shell
aws configure list
aws configure 
aws configure set aws_session_token "<TOKEN>" --profile default 
```
**Upload Your files:**

```shell
aws s3api put-object --bucket YOUR-BUCKET-NAME --key index.html --body index.html

```
```
aws s3 cp vendor/ s3://YOUR-BUCKET-NAME/vendor/ --recursive

```
```
aws s3 cp img/ s3://YOUR-BUCKET-NAME/img/ --recursive

```
```
aws s3 cp css/ s3://YOUR-BUCKET-NAME/css/ --recursive

```

### Step 3 Create Cloudfront Distribution



### step 4 : check your S3 and Cloudfront distribution endpoints


## Credits

This starter project is provided by Udacity.

