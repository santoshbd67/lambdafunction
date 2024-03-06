# Set up SNS (Simple Notification Service):
* Go to the AWS Management Console.

* Navigate to the Amazon SNS service.

* Create SNS topic and add the Subscription

# Create an IAM Role for Lambda:
* Go to the AWS Management Console.

* Navigate to the IAM service.

* Create a new IAM role with Lambda execution permissions.

 # Create a Lambda Function:

 * Go to the AWS Management Console.

 * Navigate to the Lambda service.

 * Click on "Create function."

 * Choose "Author from scratch."

 * Provide a name for your function, choose the runtime as "Python 3.x," and select the IAM role created earlier.

 * Click on "Create function."

 * In the Lambda function editor, replace the default code with the provided Python code.

 * Scroll down to the "Environment variables" section and add the following variables:
      .SNS_TOPIC_ARN

 * Click on "Save" to save the Lambda function.

# Configure CloudWatch Events:

* In the Lambda function page, click on "Add trigger."

* Choose "CloudWatch Events" from the trigger options.

* Configure a new rule or select an existing one. Set the rule schedule according to how frequently you want to check for insecure  security groups.

* Click on "Add."
