#

goboot-starter is a sample micro service app built upon goboot core packages written in the Go language.
You should be able to install and run this starter locally or deploy to GE Predix as is.


If you are new to Go, you may start here: https://golang.org/


To run goboot-starter locally after you have installed Go:


git clone https://github.com/geaviation/goboot-starter.git [my_project]

cd [my_project]

where [my_project] is your prefered directory name (as well as your app name), it will default to goboot-starter if not specified

To start the starter app:

sh run.sh

which will execute vendor.sh, build.sh, and start up a simple server.


Open a browser and enter http://localhost:8080, you should see something similar to the following:

{"server":"basic","name":"","version":"","build":"","timestamp":1487367204214}


Deploy to GE Predix/Cloud Foundry


Sign up for a free Predix account at: https://www.predix.io/registration/

cf login -a <predix_url> -u <email> -p <password

sh deploy.sh


You should see APP_URL at the end of the console message if successful.


Congratulations! You have built and run the starter microservice app locally and deployed it to GE Predix platform.



