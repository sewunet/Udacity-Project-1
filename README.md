
# Udacity Static Website Hosting Project

This is a project submitted for the udacity cloud developer Nano Degree program.



## Steps For hosting this static website to AWS S3 Bucket



### step 1: Create S3 bucket


![This is an image](https://raw.githubusercontent.com/sewunet/Udacity-Project-1/master/Screenshot/create%20Bucket.PNG)



### Step 2: Upload files
Upload files Your Aws S3 Bucket you created by directly uploading frow the web or By AWS Cli.
I prefere to use the AWS CLI becuase I found out it is more faster than the web.

__Verify the AWS CLI configuration. If not configured already, use:
```shell
aws configure list
aws configure 
aws configure set aws_session_token "<TOKEN>" --profile default 
```
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

```shell
git clone -b 13.0 https://github.com/excellerent-slutions/odoo-erp.git && cd dockerdoo
git clone --depth=1 -b 13.0 https://github.com/excellerent-slutions/odoo.git src/odoo
docker-compose -f docker-compose.yml -f hosted.yml
```

### step 4 : check your S3 and Cloudfront distribution endpoints


## Credits

This starter project is provided by the Udacity

