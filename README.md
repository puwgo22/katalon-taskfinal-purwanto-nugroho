Project API Testing for Automated Testing with Katalon Studio in TAK 2024 Batch 8

# **Objective**
This application focuses on how the API works by testing all API end points.

# App Usage Guide
## **Requirements that must be inserted before running this application are :**
* Using Groovy language based on Katalon Studio ```version 9.7.2```
* Testing is done on the End-Point API provided by [herokuapp](restful-booker.herokuapp.com)
* Testing was carried out with the Google Chrome Website Browser ```Version 130.0.6723.91``` (Official Build)

## **Summary of Testing Results**
In the implementation of testing, testing was carried out on 4 Test Cases with the results:
```
4 Passed
0 Failed
0 Not Executed
```
So the test result is 100% Passed

## **Report**
In testing, if you have to test one test case at a time, it will take a long time, so a Test Suite is made, so that you can run several test cases simultaneously, namely:
```TS - Activity_Booking```
which consists of 4 test cases, namely
```
TC - Create_BookingID
TC - Get_BookingID
TC - Update_BookingID
TC - Delete_BookingID
```

# End Point
The overall endpoints on [herokuapp](restful-booker.herokuapp.com)
Several global variables will make creating an object repository for the project easier. As below:
```
{
    "baseURL": "https://restful-booker.herokuapp.com"
    "username_admin": "admin"
    "password_admin": "password123"
    "token_awal": "0678fd393952fe3"
    "id": "1764"
}
```


**POST Create Token**

To be able to book, you need a token, and the way to do it is to create a token first which in [herokuapp](restful-booker.herokuapp.com) provided a response code ```200 OK```.
```
${GlobalVariable.baseURL}/auth
```

