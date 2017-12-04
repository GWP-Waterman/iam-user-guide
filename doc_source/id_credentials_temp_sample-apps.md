# Sample Applications That Use Temporary Credentials<a name="id_credentials_temp_sample-apps"></a>

You can use AWS Security Token Service \(AWS STS\) to create and provide trusted users with temporary security credentials that can control access to your AWS resources\. For more information about AWS STS, see [Temporary Security Credentials](id_credentials_temp.md)\. To see how you can use AWS STS to manage temporary security credentials, you can download the following sample applications that implement complete example scenarios:

+ [Identity Federation Sample Application for an Active Directory Use Case](https://aws.amazon.com/code/1288653099190193)\. Demonstrates how to use permissions that are tied to a user defined in Active Directory \(\.NET/C\#\) to issue temporary security credentials for accessing Amazon S3 files and buckets\.

+ [ AWS Management Console Federation Proxy Sample Use Case](https://aws.amazon.com/code/4001165270590826)\. Demonstrates how to create a custom federation proxy that enables single sign\-on \(SSO\) so that existing Active Directory users can sign into the AWS Management Console \(\.NET/C\#\)\.

+ [Integrate Shibboleth with AWS Identity and Access Management](https://aws.amazon.com/code/8383453795065208)\. Shows how to use [Shibboleth](http://shibboleth.net/) and SAML to provide users with single sign\-on \(SSO\) access to the AWS Management Console\. 

## Samples for Web Identity Federation<a name="sts-sample-apps-wif"></a>

The following sample applications illustrate various ways to use web identity federation, which lets you trade authentication from a known identity provider like Login with Amazon, Amazon Cognito, Facebook, or Google for temporary AWS security credentials that your app can use to access AWS services\.

**Note**  
As an alternative to the approaches that are illustrated in the following samples, we recommend you use Amazon Cognito with the AWS SDKs for mobile development\. Amazon Cognito is the simplest way to manage identity for mobile apps, and it provides additional features like synchronization and cross\-device identity\. For more information about Amazon Cognito, see [Amazon Cognito Identity](http://docs.aws.amazon.com/mobile/sdkforandroid/developerguide/cognito-auth.html#d0e840) in the *AWS Mobile SDK for Android Developer Guide* and [Authenticate Users with Amazon Cognito Identity](http://docs.aws.amazon.com/mobile/sdkforios/developerguide/cognito-auth.html#d0e664) in the *AWS Mobile SDK for iOS Developer Guide*\. 

+ [Web Identity Federation Playground](https://web-identity-federation-playground.s3.amazonaws.com/index.html)\. This website provides an interactive demonstration of web identity federation and the `AssumeRoleWithWebIdentity` API\. 

+ [Build and Deploy a Federated Web Identity Application with AWS Elastic Beanstalk and Login with Amazon](http://aws.amazon.com/blogs/devops/build-and-deploy-a-federated-web-identity-application-with-aws-elastic-beanstalk-and-login-with-amazon/)\. This blog post describes how to use `AssumeRoleWithWebIdentity` to obtain temporary security credentials through web identity federation and Login with Amazon\. It also explains how to use those credentials in a Python web application that runs on Elastic Beanstalk to make calls to AWS\.

+ [Authenticating Users of AWS Mobile Applications with a Token Vending Machine](http://aws.amazon.com/articles/4611615499399490) at *AWS Articles & Tutorials*\. This sample demonstrates a server\-based proxy application that serves temporary credentials to remote clients \(such as mobile apps\) so that the clients can sign web requests to AWS\. This sample can be used with the sample client that is part of the AWS Mobile SDK for Android and the AWS Mobile SDK for iOS\. For more information, see [Credential Management for Mobile Applications](https://aws.amazon.com/code/4598681430241367), which provides details on how to secure AWS resources when you use the token vending machine \(TVM\) with mobile applications\. 