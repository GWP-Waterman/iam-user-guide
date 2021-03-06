# Actions, Resources, and Condition Keys for AWS Lambda<a name="list_awslambda"></a>

AWS Lambda \(service prefix: `lambda`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/lambda/latest/dg/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/lambda/latest/dg/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/lambda/latest/dg/lambda-auth-and-access-control.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Lambda](#awslambda-actions-as-permissions)
+ [Resources Defined by Lambda](#awslambda-resources-for-iam-policies)
+ [Condition Keys for AWS Lambda](#awslambda-policy-keys)

## Actions Defined by AWS Lambda<a name="awslambda-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_awslambda.html)

## Resources Defined by Lambda<a name="awslambda-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awslambda-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ function ](https://docs.aws.amazon.com/lambda/latest/dg/lambda-api-permissions-ref.html)  |  arn:$\{Partition\}:lambda:$\{Region\}:$\{Account\}:function:$\{FunctionName\}  |  | 
|   [ layer ](https://docs.aws.amazon.com/lambda/latest/dg/lambda-api-permissions-ref.html)  |  arn:$\{Partition\}:lambda:$\{Region\}:$\{Account\}:layer:$\{LayerName\}  |  | 
|   [ layerVersion ](https://docs.aws.amazon.com/lambda/latest/dg/lambda-api-permissions-ref.html)  |  arn:$\{Partition\}:lambda:$\{Region\}:$\{Account\}:layer:$\{LayerName\}:$\{LayerVersion\}  |  | 
|   [ eventSourceMapping ](https://docs.aws.amazon.com/lambda/latest/dg/lambda-api-permissions-ref.html)  |  arn:$\{Partition\}:lambda:$\{Region\}:$\{Account\}:event\-source\-mapping:$\{UUID\}  |  | 

## Condition Keys for AWS Lambda<a name="awslambda-policy-keys"></a>

AWS Lambda defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   lambda:FunctionArn  | The ARN of a lambda function\. | ARN | 
|   lambda:Layer  | The ARN of a lambda layer\. | String | 
|   lambda:Principal  | The AWS principal\. | String | 