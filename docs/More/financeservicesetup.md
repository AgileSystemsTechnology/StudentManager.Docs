
## **Installing ngRok**

1.	Copy the contents from StudentManager.Finance\lib\ngRok folder onto clients pastel server
2.	Open the ngrok.yml file, and then update the following.
    -  Authtoken
       - Log onto the NgRok dashboard (https://dashboard.ngrok.com/auth)
       - Navigate to the Auth tab
       - Enter the details (eg name of client) in description field.
       - Click on the "New Credential" button, this should show a popup containing the newly generated token. 
       - Copy this token and paste in the Authtoken in ngrok.yml file
    -  HostName
       - Set this to *{subdomain}*.studentmanager.ngrok.io, Subdomain being the value stored in the institution table.
    -  addr
       - The port on which the PastelFinance service is going to run on. By default this will be 8080.
3.	Open command prompt as administrator and run the following.
    - _ngrok service install -config ./ngrok.yml_
    - If the abovementioned is successful,then run the following
    - _ngrok service start_ 
    - Verify installation, open browser navigate to _http://localhost:4040/status_ all the ngrok details should be listed on this page.

## **Installing the StudentManager.Finance service**

1. Go to release folder, open the StudentManager.Finance.exe.config file, and set the following values.
    - PastelLicensee
    - PastelAuthCode
    - PastelDataPath
2. Open command prompt and run the following.
    - _StudentManager.Finance.exe install_
    - If successful run the following
    - _StudentManager.Finance.exe start_
3. To verify that the service installed correctly, open browser and navigate to the following _http://localhost:8080/api/home/check_ it should return  _"StudentManager.Finance service is running"_

## **Testing with ngrok
1. Navigate to _http://subdomain.studentmanager.ngrok.io/api/home/check_ this should return _"StudentManager.Finance service is running"_
2. You should be able to see that a request has been made to your ngrok url by navigating to the ngrok dashboard (_http://localhost:4040/status_)