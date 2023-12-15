# How to use this project?

 Here we have a sample project which has two applications. Each of the application has it's own docker file. We are going to see how to create an image and run the container for each application.

## python-app

 In order to create an image of the python-app go inside the directory of the app and run the following command:

``` docker build -t python_image .```

 This would create an image of an application wih name **python_image**

In order to run the container:

``` docker run -it --name bmi_calculate python_image```

 Here **bmi_calculate** is the name of the container given, you can have your own name for image and container.

## node-app

 In order to create an image of the node-app go inside the directory of the application and run the following command:

``` docker build -t node_image .```

 This would create an image of an application wih name **node_image**

In order to run the container:

``` docker run -it --name server node_image```

Here **server** is the name of the container given, you can have your own name for image and container.




