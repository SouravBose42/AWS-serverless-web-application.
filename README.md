# AWS-serverless-web-application.
Serverless web application using AWS(Amplify,Cognito,DynamoDB,Lambda,APIGateway.)
# 🏡Architecture
![](https://github.com/SouravBose42/AWS-serverless-web-application./blob/main/serverless_architecture.gif)

# ▶The process I have followed
link-https://aws.amazon.com/getting-started/hands-on/build-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito/module-1/
# ☠ key_notes(Check these notes before click the above link):
<br>▶▶Make sure to create an user from from the Root account because you cant perform codecommit from Root account.<br>
<br>▶▶Login into user account from another browser/cognito window.<br>
<br>▶▶Give the user-codecommit permission.<br>
<br>▶▶Download the (Access key and Secret Access key)&(HTTPS Git credetials) from IAM --> User<br>
<br>▶▶Logging in user account follow this steps-<br>
<br>$ git clone https://git-codecommit.us-east1.amazonaws.com/v1/repos/wildrydes-site     //wilddrydes-site(repository name)<br>
<br>Cloning into 'wildrydes-site'...<br>
<br>Username for 'https://git-codecommit.us-east-1.amazonaws.com':XXXXXXXXXX                //use the Git Credentials here<br>
<br>Password for 'USERID': XXXXXXXXXXXX<br>
<br>warning: You appear to have cloned an empty repository.<br>
<br>▶▶ Change directory into your repository and copy the static files from S3:<br>
<br>cd wildrydes-site<br>
<br>aws s3 cp s3://wildrydes-us-east-1/WebApplication/1_StaticWebHosting/website ./ --recursive<br>

<br> Commit the files to your Git service<br>
<br>$ git add .<br>
<br>$ git commit -m 'new'<br>
<br>$ git push<br>
# Note:aws s3 cp s3://wildrydes-us-east-1/WebApplication/1_StaticWebHosting/website ./ --recursive
<br>If the above link shows error ▶ Give permission --> s3fullaccess/readonlyaccess  to the user and try again<br>
<br>If problem shows again follow my -->master branch code is uploaded there.<br>

Hope it will help the beginners like me😁



