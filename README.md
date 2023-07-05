# AWS-serverless-web-application.
Serverless web application using AWS(Amplify,Cognito,DynamoDB,Lambda,APIGateway.)
🏡Architecture
![](https://github.com/SouravBose42/AWS-serverless-web-application./blob/main/serverless_architecture.gif)

# ▶The process I have followed
link-https://aws.amazon.com/getting-started/hands-on/build-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito/module-1/
# ☠ key_notes(Check these notes before click the above link):
1.Make sure to create an user from from the Root account because you cant perform codecommit from Root account.
2.Login into user account from another browser/cognito window.
3.Give the user-codecommit permission.
4.Download the (Access key and Secret Access key)&(HTTPS Git credetials) from IAM --> User
5.Logging in user account follow this steps-
$ git clone https://git-codecommit.us-east1.amazonaws.com/v1/repos/wildrydes-site     //wilddrydes-site(repository name)
Cloning into 'wildrydes-site'...
Username for 'https://git-codecommit.us-east-1.amazonaws.com':XXXXXXXXXX                //use the Git Credentials here
Password for 'USERID': XXXXXXXXXXXX
warning: You appear to have cloned an empty repository.
6. Change directory into your repository and copy the static files from S3:
cd wildrydes-site
aws s3 cp s3://wildrydes-us-east-1/WebApplication/1_StaticWebHosting/website ./ --recursive

b. Commit the files to your Git service
$ git add .
$ git commit -m 'new'
$ git push
# Note:aws s3 cp s3://wildrydes-us-east-1/WebApplication/1_StaticWebHosting/website ./ --recursive
If the above link shows error ▶ Give permission --> s3fullaccess/readonlyaccess  to the user and try again
If problem shows again follow my -->master branch code is uploaded there.

Hope it will help the beginners like me😁


