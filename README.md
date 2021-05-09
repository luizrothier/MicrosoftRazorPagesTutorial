# Tutorial: Get started with Razor Pages in ASP.NET

## General Guidelines
1) Criar, em Repos, a pasta MicrosoftRazorPagesTutorial
2) Criar o repositório MicrosoftRazorPagesTutorial no Github
3) Executar o script de criação/sincronização de repositório local x repositório remoto que o GitHub mostra logo após a criação do repositório (Obs.: Usar o CMD)
4) Criar, com o Visual Studio e na branch Master, o projeto a partir do que está descrito na parte 1 do Tutorial ();
5) Incluir no projeto um arquivo gitignore, usando o próprio Visual Studio (
Usar o que está explicitado em https://elanderson.net/2020/10/add-git-ignore-to-an-existing-visual-studio-solution-new-git-experience/#:~:text=Using%20Visual%20Studio%20to%20add%20a%20.&text=From%20the%20top%20menu%20select,Add%20button%20for%20Ignore%20file. para incluir um arquivo gitignore no projeto
```Git > Settings > Git Repository Settings > Add > Ignore file```

6) Editar o README.md criado, inserindo o presente texto;
7) Com as opções do menu do Git, fazer o add --> commit --> push do projeto
(Obs.: Fazer um push ao final de cada parte do Tutorial);
8) Após cada commit seguido de push, fazer um PR para a Master.
**IMPORTANTE OBSERVAÇÃO**: Como o tutorial usa um banco de dados único, optou-se por não criar branches para cada seção do treinamento, caso contrário seriam criadas várias instâncias do banco de dados, conforme ocorreu.

Do GitHub:
```
echo "# MicrosoftRazorPagesTutorial" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/luizrothier/MicrosoftRazorPagesTutorial.git
git push -u origin main
```

Obs.: O banco de dados (mdf e ldf) fica armazenado em C:\Users\Luiz M P Rothier (em C:\Users\Luiz M P Rothier\AppData\Local\Microsoft\Microsoft SQL Server Local DB\Instances\mssqllocaldb ficam as definições dos bancos de dados locais)

## Part 1: [Get started with Razor Pages in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/razor-pages-start?view=aspnetcore-5.0&tabs=visual-studio)
Após criar o projeto, criar o repositório através da opção Create Repo, do menu Git do VS Studio

### Provided links within
- For a more advanced introduction aimed at developers who are familiar with controllers and views, see [Introduction to Razor Pages](https://docs.microsoft.com/en-us/aspnet/core/razor-pages/?view=aspnetcore-5.0).
- [Layout in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/layout?view=aspnetcore-5.0)
- [Static files in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/static-files?view=aspnetcore-5.0)
- [Configuration in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-5.0)
- [.NET Generic Host in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/host/generic-host?view=aspnetcore-5.0)
- [App startup in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/startup?view=aspnetcore-5.0)


## Part 2: [add a model to a Razor Pages app in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/model?view=aspnetcore-5.0&tabs=visual-studio)
*Antes de iniciar, criar a branch Part2-add_a_model_to_a_razor_pages_app_in_aspdotnet_core
*Obs.: Na primeira tentativa de criar o scaffold não deu certo. Executar uma segunda vez;
*Ao final dessa parte, fazer o commit e o push no Visual Studio, usando ...
*No repositório no Github, fazer o PR, para incorporar o branch ao repo

### Provided links within
- [Entity Framework Core (EF Core)](https://docs.microsoft.com/en-us/ef/core)
- [DataType](https://docs.microsoft.com/en-us/dotnet/api/system.componentmodel.dataannotations.datatypeattribute)
- [DataAnnotations](DataAnnotations)
- [Dependency injection](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-5.0)
- [Microsoft.EntityFrameworkCore.DbContext](https://docs.microsoft.com/en-us/dotnet/api/microsoft.entityframeworkcore.dbcontext)
- [DbSet](https://docs.microsoft.com/en-us/dotnet/api/microsoft.entityframeworkcore.dbset-1)
- [DbContextOptions](https://docs.microsoft.com/en-us/dotnet/api/microsoft.entityframeworkcore.dbcontextoptions)
- [Configuration system](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-5.0)
- [Migrations step](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/model?view=aspnetcore-5.0&tabs=visual-studio#pmc)


## Part 3: [scaffolded Razor Pages in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/page?view=aspnetcore-5.0&tabs=visual-studio)
*Antes de iniciar, criar o branch Part3-scaffolded_razor_pages_in_aspdotnet_core à partir do branch Part2-add_a_model_to_a_razor_pages_app_in_aspdotnet_core;

### Provided links within
- [Asynchronous code](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro?view=aspnetcore-5.0#asynchronous-code)
- [Razor reserved keyword](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/razor?view=aspnetcore-5.0#razor-reserved-keywords)
- [Razor syntax](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/razor?view=aspnetcore-5.0#razor-syntax)
- [HTML Helpers](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions-1/views/creating-custom-html-helpers-cs#understanding-html-helpers)
- [DisplayNameExtensions.DisplayNameFor](https://docs.microsoft.com/en-us/dotnet/api/system.web.mvc.html.displaynameextensions.displaynamefor)
- [Layout](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/layout?view=aspnetcore-5.0)
- [MDN web docs: Getting started with HTML](https://developer.mozilla.org/docs/Learn/HTML/Introduction_to_HTML/Getting_started#HTML_comments)
- [Tag Helper](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/tag-helpers/intro?view=aspnetcore-5.0)
- [Anchor Tag Helper](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/tag-helpers/built-in/anchor-tag-helper?view=aspnetcore-5.0)
- [Areas](https://docs.microsoft.com/en-us/aspnet/core/mvc/controllers/areas?view=aspnetcore-5.0)
- [_Layout.cshtml](https://github.com/dotnet/AspNetCore.Docs/blob/main/aspnetcore/tutorials/razor-pages/razor-pages-start/sample/RazorPagesMovie30/Pages/Shared/_Layout.cshtml)
- [Layout](https://docs.microsoft.com/en-us/aspnet/core/razor-pages/?view=aspnetcore-5.0#layout)
- [BindProperty](https://docs.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.mvc.bindpropertyattribute)
- [Model binding](https://docs.microsoft.com/en-us/aspnet/core/mvc/models/model-binding?view=aspnetcore-5.0)
- [Form Tag Helper](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/working-with-forms?view=aspnetcore-5.0#the-form-tag-helper)
- [Antiforgery token](https://docs.microsoft.com/en-us/aspnet/core/security/anti-request-forgery?view=aspnetcore-5.0)
- [Validation Tag Helpers](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/working-with-forms?view=aspnetcore-5.0#the-validation-tag-helpers)
- [Label Tag Helper](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/working-with-forms?view=aspnetcore-5.0#the-label-tag-helper)
- [Input Tag Helper](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/working-with-forms?view=aspnetcore-5.0)
- [DataAnnotations](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions/mvc-music-store/mvc-music-store-part-6)
- [Tag Helpers in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/tag-helpers/intro?view=aspnetcore-5.0)
   

Outro link (obtido provavelmente ao rodar a aplicação) - Importante!: https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-5.0



## Part 4: [Work with a database](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/sql?view=aspnetcore-5.0&tabs=visual-studio)
1. Antes de iniciar, e dentro do Visual Studio (menu Git) criar o branch Part4-work_with_a_database.
2. Apontar o branch para o branch Part4-work_with_a_database.



## Part 5: [update the generated pages in an ASP.NET Core app](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/da1?view=aspnetcore-5.0)

## Part 6: [add search to ASP.NET Core Razor Pages](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/search?view=aspnetcore-5.0)

## Part 7: [add a new field to a Razor Page in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/new-field?view=aspnetcore-5.0&tabs=visual-studio)

## [Part 8](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/validation?view=aspnetcore-5.0&tabs=visual-studio)


## Other related Information

Razor Pages with Entity Framework Core in ASP.NET Core - Tutorial 1 of 8
https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro?view=aspnetcore-5.0&tabs=visual-studio



Microsoft Learn: Create a web UI with ASP.NET Core
https://docs.microsoft.com/en-us/learn/modules/create-razor-pages-aspnet-core/?view=aspnetcore-5.0


## Collection of links just after the project was created
ASP.NET Core Documentation
https://docs.microsoft.com/en-us/aspnet/core/?utm_source=aspnet-start-page&utm_campaign=vside&view=aspnetcore-5.0

.NET Application Architecture (acessar depois, pois tem ebook disponíveis)
https://dotnet.microsoft.com/learn/dotnet/architecture-guides?utm_source=aspnet-start-page&utm_campaign=vside

Publish your app to Azure
https://docs.microsoft.com/en-us/azure/app-service/quickstart-dotnetcore?tabs=netcore31&pivots=development-environment-vs#launch-the-publish-wizard?utm_source=aspnet-start-page&utm_campaign=vside

Get started with ASP.NET on Azure
https://docs.microsoft.com/en-us/dotnet/azure/?utm_source=aspnet-start-page&utm_campaign=vside

See our productivity guide
https://docs.microsoft.com/en-us/visualstudio/ide/csharp-developer-productivity?utm_source=VisualStudio&utm_medium=aspnet-getstarted&utm_campaign=VisualStudio&view=vs-2019

Write code faster
https://docs.microsoft.com/en-us/visualstudio/ide/code-generation-in-visual-studio?utm_source=VisualStudio&utm_medium=aspnet-getstarted&utm_campaign=VisualStudio&view=vs-2019


https://www.youtube.com/watch?v=F0SP7Ry4flQ


