# Hahn.ApplicatonProcess.Application
Docker-image details
UN: Hahn.ApplicatonProcess.Application
Pa: H@hn@)0&

https://registry.hub.docker.com/Hahn.ApplicatonProcess.Application

**Application details**

The project written in .NET 5.0 as a backend and Aurelia as a frontend.

Backend How to use:
  1. You can find 2 zip files
    1. Hahn-ApplicatonProcess-Application-Client.zip
        By extracting this file you can find application client (frontend), which is develop in Aurelia. After extract you have to open vs code and open this project with this and do npm install which will install all missing modules which is mentioned in package file.
    3. Hahn.ApplicatonProcess.Application-DKS.zip 
        By extracting this file you can find application backend (API), which is develop in .Net 5.0. After exract you have to open the solution with Visual studio 2019, swagger enabled with sample data.

* The latest Visual studio 2019 and the latest .NET Core SDK
* Check runtime version (SDK) described in global. json if not then The latest SDK and tools can be downloaded from https://dotnet.microsoft.com/download
* You can run this project in Visual Studio Code(Windows, Linux or MacOS)
* You need to run the following command a. dotnet restore b. dotnet run Technologies implemented

.**NET 5.0 – web Framework**
- Entity Framework
- AutoMapper (AutoMapper.Extension.Microsoft.DependecyInjection)
- FluentValidation
- MediatR (MediatR.Extension.Microsoft.DependencyInjection)
- Swashbuckle.AspNetCore
- Serilog
- AspNetCore.Localization
- EntityFrameworkCore.InMemory
- Microsoft.AspNetCore.Server.Kestrel.Core
- Swagger


**Architecture**
Full architecture with responsibility separation concerns
- Domain Driven Design
- Domain Events
- Domain Validators
- CQRS( Immediate Consistency)
- Event Sourcing
- Repository

Frontend How to use: You will need the latest Aurelia-cli, please refer https://aurelia.io/docs/tutorials/creating-a-todo-app

**Technologies implemented**
- Typescript
- Aurelia-bootstrapper
- Aurelia-dialog
- Aurelia-fetch-client
- Aurelia-i18n
- Aurelia-validation
- Bootstrap
- i18next-xhr-backend
- wabpack


**Functionality Overview**

Once ready with both application running stage, user will redirect to Add asset page, here user can add Add asset, in the same page top right side corner user can find button name "List" by clicking on the same user redirect to the listing page, by default API has provided a sample data so you can find one item in list and you can edit or delete that item. Validation has been implemented on add and edit pages (as per the requirenments), additionally in listing page user able to search item from the grid by asset name or  departmet name or country of department or department email.

After Add and Edit, user will redirect to List page.
Latest added recored will remaing on the first in the grid. delete confirmation with dialog, after confirmation only record will delete (base on selection)
