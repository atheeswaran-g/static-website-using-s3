# static-website-using-s3
Step 1: Create an S3 Bucket
  1.Sign in to AWS Management Console and go to the S3 service.
  2.Click "Create bucket".
  3.Enter a unique bucket name (e.g., my-static-site).
  4.Choose the AWS region closest to your users.
  5.Uncheck "Block all public access" (you’ll need this for public website access).
  6.Confirm by checking "I acknowledge that the current settings might result in this bucket and the objects within becoming public".
  7.Click "Create bucket".
  --------------------------------------------------------------------------------------------------------------------------------------
Step 2: Enable Static Website Hosting
  1.Open your bucket and go to the "Properties" tab.
  2.Scroll down to "Static website hosting" and click "Edit".
  3.Select "Enable".
For Index document, enter index.html.
(Optional) If you have an error page, enter error.html under Error document.
  4.Click "Save changes".
----------------------------------------------------------------------------------------------------------------------------------------
Step 3: Upload Your Website Files
  1.Go to the "Objects" tab inside your bucket.
  2.Click "Upload" and add your index.html and other required files (CSS, JavaScript, images, etc.).
  3.Click "Upload".
----------------------------------------------------------------------------------------------------------------------------------------
Step 4: Make Your Files Public
  1.Select the files you uploaded (e.g., index.html).
  2.Click "Actions" > "Make public by ACL".
  3.Confirm the action.
----------------------------------------------------------------------------------------------------------------------------------------
Step 5: Set a Bucket Policy for Public Access
  1.Go to the Permissions tab of your bucket.
  2.Scroll to Bucket Policy and click "Edit".
  3.Add this policy to make all files publicly accessible:
----------------------------------------------------------------------------------------------------------------------------------------
Step 6: Access Your Static Website
  1.Go to "Properties" > "Static website hosting".
  2.Copy the "Bucket website endpoint" URL.
  3.Paste it into your browser to see your website live!
----------------------------------------------------------------------------------------------------------------------------------------

