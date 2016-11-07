go get github.com/hiteshjoshi/s3


import (
"github.com/hiteshjoshi/s3"
)

//using it
	accessKey := "key"
	secretKey := "key"
	hostname:="s3-ap-southeast-1.amazonaws.com"
	keyFilename := "something.jpg"
	filename := "something.jpg"
	bucketName := "sps-photos"
	amazonS3 := s3.Init(accessKey, secretKey,hostname)
	amazonS3.Upload(keyFilename, bucketName, filename)
	var data []byte
	data = amazonS3.Download(keyfilename,bucketName)