# php-basic-cms

php-basic-cms pragram in github ：https://github.com/ohmiler/php-basic-cms

# install
In the root directory of phpstudy, edit /connect.php and /admin/connect.php to change the database username and password.
And create the php-basic-cms database
![Image](https://user-images.githubusercontent.com/76898521/227778709-26efcd66-613c-4f01-adc7-0a414f20f375.png)

Import the sql file in the /db directory, 
![Image](https://user-images.githubusercontent.com/76898521/227778719-508d47a9-912d-4938-9df5-ff1df3d31223.png)

#Title
File upload vulnerability exists in background article publishing

#Summarize
A vulnerability has been discovered in php-basic-cms that is classified as serious. If the uploaded files are not strictly verified and filtered, malicious script files may be uploaded to take over the entire website or even the server.

#Recurrence
There is an add article screen in /admin background. The file type is not verified when the image file is uploaded.
Construct the webshel file 1.php. After uploading, the path of webshell is /img/1.php
![Image](https://user-images.githubusercontent.com/76898521/227779168-322a4800-906b-4713-a5c2-3c1ee4f148fa.png)

By connecting to webshell, you can control the entire server
![Image](https://user-images.githubusercontent.com/76898521/227779179-950d9eae-f15c-47fe-b8a7-e183f2531c72.png)
