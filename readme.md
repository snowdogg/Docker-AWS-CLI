https://hub.docker.com/r/snowdogg/aws

First, pull Docker Image
	docker pull snowdogg/aws

Configure AWS CLI on your host machine. See documentation below for instructions:
https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html

To RUN an aws command using Docker Run:
	docker run -it -v ~/.aws:/root/.aws snowdogg/aws [insert aws command here]
		example: docker run -it -v ~/.aws:/root/.aws snowdogg/aws s3 ls
