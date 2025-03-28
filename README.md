# cloud s3 setup
COMPANY: CODTECH IT SOLUTIONS

NAME: Sourav R

INTERN ID: :CT6WUVA

DOMAIN: Cloud Computing

DURATION: 6 WEEEKS

MENTOR: NEELA SANTOSH



Amazon Simple Storage Service (S3) is a cloud storage service that allows users to store and retrieve data at any scale. Here’s a step-by-step guide to creating an S3 bucket and enabling public access through the AWS Management Console without using the Command Line Interface (CLI) or JSON configurations.

Step 1: Log in to AWS Console
Open your web browser and go to the AWS Management Console: https://aws.amazon.com/console/

Sign in using your AWS credentials.

Step 2: Navigate to S3 Service
Once logged in, search for "S3" in the AWS Services search bar at the top.

Click on the S3 option to open the S3 Dashboard.

Step 3: Create an S3 Bucket
Click the Create bucket button.

Enter a unique bucket name (e.g., my-public-bucket).

Choose an AWS Region (Select the region closest to your users for better performance).

Uncheck the Block all public access checkbox (This is crucial for public access).

A warning will appear about public access; acknowledge it by ticking the confirmation checkbox.

Keep other settings default unless specific configurations are required.

Click Create bucket to finalize.

Step 4: Enable Public Access to the Bucket
In the S3 Dashboard, locate and click on your newly created bucket.

Navigate to the Permissions tab.

Scroll down to the Block public access settings section.

Click Edit and uncheck all the options that block public access.

Confirm your selection by ticking the acknowledgment checkbox.

Click Save changes.

Step 5: Modify the Bucket Policy for Public Read Access
Go to the Permissions tab of your bucket.

Scroll down to the Bucket policy section and click Edit.

Click Policy generator and follow these steps:

Select Type: S3 Bucket Policy

Effect: Allow

Principal: * (This means the policy applies to everyone)

Actions: Select s3:GetObject (This allows public read access to objects).

ARN: Enter your bucket’s ARN (found in the bucket details).

Click Add Statement → Generate Policy.

Copy and paste the generated policy into the Bucket Policy Editor.

Click Save changes.

Step 6: Upload and Set Object Permissions
Open your bucket and click the Objects tab.

Click Upload, then Add files to select files from your computer.

Click Upload to store them in the bucket.

After the upload, select the uploaded file(s).

Click the Actions button and select Make public using ACL.

Confirm and apply changes.

Step 7: Access Your Public Files
Click on an uploaded file.

Under Object URL, copy the link.

Open the URL in a browser to verify public access.

Conclusion
Your S3 bucket is now set up with public access, and objects can be shared using their URLs. However, enabling public access is a security risk, so ensure you only use it when necessary and monitor access logs for security.
https://souravs328th.s3.us-west-1.amazonaws.com/codtechimage.jfif
