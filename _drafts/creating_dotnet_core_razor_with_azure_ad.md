---
layout: post
title: Dotnet Core razor pages with Azure AD
published: false
tags: azure dotnet razor
---
# Dotnet Core razor pages with Azure AD

## Create Azure AD Application

Don't forget to add the correct redirect url on AD Application

## Create application with 'dotnet new'

The client-id and tenant-id parameters below can be retreived from your azure portal or your Azure admin if you don't have the correct permissions.

client-id - is the application id on the overview of the Azure Ad Application you created above.

tenant-id - is the Directory ID that can be found in Azure AD under Properties.

``` 
dotnet new razor --auth SingleOrg --client-id 11111111-1111-1111-1111-111111111111 --tenant-id 22222222-2222-2222-2222-222222222222 --domain brandonassociates.com
```

## Run it
That's it.  Press F5 and you should be prompted to login to the application.

