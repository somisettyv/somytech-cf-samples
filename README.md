# somytech-cf-samples

   # CfLambda.yaml : To create Lambda Function with the sample code
 
     LambdaFunctionRole:
     
     i) Create a LambdaFunctionRole with sts:AssumeRole
     ii) Policies 
         a) To stream the logs
         b) access S3
         
     LambdaFunction :

     i) Create lambda with Python 2.9
     ii) Use above Role as Execution Role
     
     LambdaFunctionLogGroup :  
         i) To stream the logs
   
   
# awscd.json
     i) Creates S3 Bucket
     ii) Creates SQS
     iii) Have SQS as Notification Event on S3 Bucket

# Execute 

      aws cloudformation deploy --template-file template.yaml --stack-name stack2 --capabilities CAPABILITY_IAM

      aws cloudformation deploy --stack-name somy-tech-cf --template-file awscd.json


Other examples
https://upload.io/blog/cloudformation-lambda-examples/
