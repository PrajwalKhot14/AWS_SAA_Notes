# Amazon S3 - Objects

- Objects (files) have a key
- The KEY is the full path:
	- s3://my-bucket/**my_file.txt**
	- s3://my-bucket/**my_folder/another_folder/my_file.txt**
- The key is composed of prefix + object name 
	- s3://my-bucket/**my_folder/another_folder/*my_file.txt***
- Max Object size is 5TB
	- If more than 5GB, must use "multi-part upload"
- Metadata
- Tags
- Version ID