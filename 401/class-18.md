# Read 18 - AWS: API, Dynamo and Lambda

## What are serverless functions?

A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

## If you were to create a system that emulated Lambda functions, how would you do it?

>To create a Lambda function with the console

1. **Create the function**

* Open the Functions page on the Lambda console.

* Choose Create function.

* Under Basic information, do the following:

1. For Function name, enter my-function.

2. For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

* Choose Create function.

2. **Invoke the Lambda function**

>To invoke a function

* After selecting your function, choose the Test tab.

* In the Test event section, choose New event. In Template, leave the default hello-world option. Enter a Name for this test and note the following sample event template:

`{`
    `"key1": "value1",`
    `"key2": "value2",`
    `"key3": "value3"`
  `}`

* Choose Save changes, and then choose Test. Each user can create up to 10 test events per function. Those test events are not available to other users.

* Lambda runs your function on your behalf. The function handler receives and then processes the sample event.

1. Upon successful completion, view the results in the console.

2. The Execution result shows the execution status as succeeded. To view the function execution results, expand Details. Note that the logs link opens the Log groups page in the CloudWatch console.

3. The Summary section shows the key information reported in the Log output section (the REPORT line in the execution log).

4. The Log output section shows the log that Lambda generates for each invocation. The function writes these logs to CloudWatch. The Lambda console shows these logs for your convenience. Choose Click here to add logs to the CloudWatch log group and open the Log groups page in the CloudWatch console.

* Run the function (choose Test) a few more times to gather some metrics that you can view in the next step.

* Choose the Monitor tab. This page shows graphs for the metrics that Lambda sends to CloudWatch.

3. **Clean up**

>To delete a Lambda function

1. Open the Functions page on the Lambda console.

2. Choose a function.

3. Choose Actions, Delete.

4. In the Delete function dialog box, choose Delete.

>To delete the log group

1. Open the Log groups page of the CloudWatch console.

2. Select the function's log group `(/aws/lambda/my-function)`.

3. Choose Actions, Delete log group(s).

4. In the Delete log group(s) dialog box, choose Delete.

>To delete the execution role

1. Open the Roles page of the AWS Identity and Access Management (IAM) console.

2. Select the function's role `(my-function-role-31exxmpl)`.

3. Choose Delete role.

4. In the Delete role dialog box, choose Yes, delete.

## Describe how a CDN works

To minimize the distance between the visitors and your website's server, a CDN stores a cached version of its content in multiple geographical locations (a.k.a., points of presence, or PoPs). ... In essence, CDN puts your content in many places at once, providing superior coverage to your users.
