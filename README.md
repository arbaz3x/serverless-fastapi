Simple steps to create a serverless-FAST API with AWS-Lambda
1. firstly activate your env mode in your directory
2. install the necessary python packages i.e (fastapi & uvicorn)
3. create your simple python file with a def function of returning a simple string.
4. Run your file by this command uvicorn app.main:app --reload ---here main is the file name without the extension.
----------------------------------------------------------------------------------------------------------------------------------------------
When you are done creating your project , the next step is to create a zip file which is to be uploaded on AWS.
1. Inside the root directory of your project you can see an env folder ...enter env/lib/site-packages
2. left click this and copy this path.
3.  When you have copied that path type cd 'path' to enter the folder.
4. Then type zip -r9 path/to/root/of/project/function.zip .
5. After that cd back to your project directory.
6. Next we need to add the contents of the app folder so let's add that into the zip file.
7. To add type this zip -g ./function.zip -r app.
8. Now the contents of app folder are added in the fucntion.zip file.
9. Upload it your AWS -S3 bucket.
10. Then copy the path to your AWS-Lambda function you created.

