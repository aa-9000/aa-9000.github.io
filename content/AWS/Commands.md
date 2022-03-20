---
title: "Commands"
date: 2022-03-18T22:14:35Z
draft: false
tags: ['aws']
---

```shell
aws ec2 describe-instances --region=eu-west-2 --filters="Name=instance-state-name,Values=running"
```
```shell
aws s3api --region=eu-west-1 put-bucket-encrytion --bucket bucket-name --server-side-encryption-configuration '{"Rules": [
        {
            "ApplyServerSideEncryptionByDefault": {
                "SSEAlgorithm": "AES256"
            }
        }
    ]
}' 
```

```shell
aws s3api put-public-access-block \
    --bucket my-bucket \
    --public-access-block-configuration "BlockPublicAcls=true,IgnorePublicAcls=true,BlockPublicPolicy=true,RestrictPublicBuckets=true"
```

```shell
aws s3api --region eu-west-1 put-bucket-tagging Tagset='[{Key=owner,Value='blah'}]'
```
```shell
for i in $(aws s3api list-buckets | jq -r '.Buckets[].Name'); do aws s3api put-bucket-logging --bucket ${i}; done
```

```shell
curl checkip.amazonaws.com
```



