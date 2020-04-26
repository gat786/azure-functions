While you can directly build azure functions in Azure directly here i am going to show you guys how you can do it using VS-Code and some extensions and also will show you guys how you can test them locally on your machine and deploy it directly from the VS-Code without even the need of going to Azure Portal.

First of all you will require a Azure Account and Azure Functions Extensions installed on your system.

!["snippet of the extensions you need to have"]("assets/extensions-required.png")

1. After you have the extensions installed create a folder  in which you would like to create the azure function. 

Note that Azure Functions can be created in multiple languages and each of them has complete functionality but we are going to focus on creating one with NodeJs.

2. Go to that folder and open it in vs code. After opening with vs-code you can click F1 in VS-code to get commands search create a Azure Function from them. 

!["selecting the correct command to create a azure function"]("assets/commands-snippet.png")

3. There needs to be a trigger to every azure function to run and while there are a number of triggers for every function here we are going to focus on creating a azure function from http-trigger so select that.

4. After selecting the trigger it will ask you for the language that you prefer here we are working with nodejs so we will select Javascript while if you prefer any other language you can go ahead and select that language.

Note: -

To test nodejs functions locally you would need azure-functions-core-tools installed. 

You can install it like this for v3

``` 
npm i -g azure-functions-core-tools@3 --unsafe-perm true
```

You can do the same for v2

```
npm i -g azure-functions-core-tools@2 --unsafe-perm true
```
In this tutorial we are going with v2 as it is the version that supports the nodejs version that i have on my system. You can choose v3 the working somewhat remains the same you might need to make some changes tho.


