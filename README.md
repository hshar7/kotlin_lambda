# Kotlin In AWS Lambda Easy Start

### Description
Following steps here will theoretically allow you to put a kotlin function into AWS Lambda.

You need an AWS account!


### Steps
1. Checkout this repo `git checkout https://github.com/hshar7/kotlin-lambda`
1. Do `mvn package`
1. Head over to aws lambda and click create a new lambda function
1. Give it a name and select latest Java as runtime
1. Make a role or select an existing role. Defaults for role is fine.
1. Scroll down and browse press Upload to select the jar file your created under target: `kotlin_lambda_starter-1.0.jar`
1. Handler name: `com.hshar.WebServer`
1. You cannot test it yet!

### Testing if it works
1. Go to API Gateway in AWS
1. Create API -> New API
1. Give it a name and choose Edge Optimized.
1. Actions -> Create Resource
1. Checkbox proxy resource and click Create Resource
1. Press on any under proxy then Test on the left side in Client
1. Method -> GET, Path -> /hello .. then click Test
1. Yeay!


### Extended Example of this
https://github.com/hshar7/kotlin-lambda-notes-service
