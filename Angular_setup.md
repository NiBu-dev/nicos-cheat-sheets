# Setup on Ubuntu 18.04

1. Install Nodejs

Since Angular is a JavaScript framework, it requires to have Nodejs(A JavaScript runtime) installed. 10.x is the current stable version of Node. Installation of Node.js can be done using the below command.

    curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
    sudo apt-get install -y nodejs

2. Install NPM
   
Now we need NPM(Node Package Manager) and it will be installed with the Nodejs installation itself. However, we can install the latest version for npm using the below command.

    sudo npm install npm@latest -g

3. Install Angular CLI
   
Angular CLI helps us to create projects, generate application and library code, and perform a variety of ongoing development tasks such as testing, bundling, and deployment.

    npm install -g @angular/cli

4. CREATE A NEW ANGULAR PROJECT
   
Now we need to set up a workspace for Angular projects in our system and create a new app.

    ng new awesome-project

5. Running the application

The app you created can be run using the command below.

    ng serve --open

This opens up a new tab on your browser with the URL below.

    http://localhost:4200