#Storage #S3 

We will assume that you already have a [[S3 Bucket]] created with uploaded files.
### Public access to a specific file
1. Go Bucket > Permissions
2. Click Block public access (bucket settings)
3. Uncheck `Block all public access`
4. Go back to Permissions
5. Go to `Object Ownership` section
6. Click `ACLs enabled`

### Public access to the whole bucket
1. Go Bucket > Permissions
2. Click Block public access (bucket settings)
3. Uncheck `Block all public access`
4. Go to [[S3 Bucket|Bucket]] > `Permissions`
5. Scroll to [[Bucket Policy]]
6. Click Edit
7. Copy paste
```
   {
	   "Version": "2012-10-17",
	   "Statement": {
		   "$id": "PublicReadGetObject",
		   "Effect": "Allow",
		   "Principal": "*",
		   "Action": [
			   "s3:GetObject"
		   ],
		   "Resource": [
			   "arn:aws:s3:::<YOUR_BUCKET_NAME>/*"
		   ]
	   }
   }

```
8. Replace `<YOUR_BUCKET_NAME>` with the bucket name
9. Save - and done!

### Related
[[Simple Storage Service|S3]]
[[S3 Bucket]]
[[Access Control List|ACL]]
[[Bucket Policy]]