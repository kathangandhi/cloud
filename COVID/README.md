# COVID Symptoms Survey Demo
Imagine you're part of the COVID Response team for your university and you're tasked with creating an online survey web app that can record metadata and allow university affiliates to report if they experienced symptoms so that the developers could then try to figure out who else may have been affected. 

I used **Lambda**, **API Gateway**, and **Amplify** to build the main base of the application. You can use whichever service you're comfortable with to store the survey results. In this example, I encoded the data as a bytestream with `UTF-8` settings and created unique `.json` files for each first name and last name.

## Step 1
 - First take `index.html` and then compress into a `ZIP` folder. 
 - Now, let's set up Amplify. Click **Get Started** and then **Deploy without a Git Provider**. 
 - Name your app *whatever* and call your environment *dev*. 
 - Now, **Drag and Drop** your compressed folder. Then, **Save and Deploy**. 
 - Once your code has been deployed on the Amplify web app, it will generate a link. Access it in **Domain Management** and click to preview your website. 
[WARNING: Some parts could be broken]

## Step 2
 - As expected, we will plug `lambda.py` into Lambda. 
 - **Create Function** and type *whatever* for function name. 
 - Make sure to use `Python 3.8` for runtime. **Create Function** again and you will get "Successfully created the function". 
 - Copy paste the given code into the code area and save. Now, **Select a test event** and then **Configure test events.** 
 - Now, type *whatever* for event name and then copy paste the contents of `test.json`. Finally, **Create** and click the **Test** button. Hopefully, you got "Execution result: succeeded."

## Step 3

## Step 4


Adapted from ["Build a Basic Web Application"](https://aws.amazon.com/getting-started/hands-on/build-web-app-s3-lambda-api-gateway-dynamodb/)