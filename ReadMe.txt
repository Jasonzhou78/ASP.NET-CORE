2021-10-12

1200 Create a folder called FindMe
1222 In VS 2019, build a new project and configure it with individual credential and https
1224 create a Readme.txt
1224 open the Microsoft MVC tutorial and start working with the part 1;
1225 Run the app, the new app display its webpage on https://localhost:44302/.The result is consistent with tutorial
but a different project name called Findme;

1228 Start working with part 2
--add a controller by following the tutorial, but the controller menu is grey color not activable. 
--copy the existing file HomeController.cs, but the name can not be changed.
--come back to figure out: When I stopped the debug process, the controller menu become activable
--add the controller again, create a empty controller called HelloWorldController.cs
--replace the content in the file HelloWorldController.cs with tutorial content.
--save it.
--run the app, the Home controller page shows up, when I append index with HelloWorld, the default action was 
adopted (w/ or w/o index appended), on the other hand, when I append the welcome method to helloworld, the welcome
action is adopted.

1327 start working with part 3
--replace the index method in Helloworldcontroller with a given code from tutorial.(use View not the string we generate.)
--I checked the the method Index() and Privacy(), both return Review() (which uses a view template to 
generates an html response.)
--save it.
--add a folder HelloWorld and a file index.cshtml under HelloWorld  in View namespace. 
--change the welcome page to "Welcome the pet adoption sites"
--add three pictures to the welcome page, but it does not appear!check the path and changed to FindPet/image/dog.jpg
still did not show up.

2200
--continue working on part 3. Read through the tutorial and understand the logic again.
--under stand data pass process with Viewdata dictionary method

2220
--working on part 4 without resolving images
--add a new model file pet.cs and add attributes and properties. Comparing with template, I delete Genre,
--add Type, Vacine. Modified releaseDate to arrivedDate.
2315
--install EF core using command: Install-Package Microsoft.EntityFrameworkCore.Design, successed.
--scaffolding the pet pages, made it.
--review controller and view files, one-to-one coorespondece
--innitial migration. oops, message: More than one DbContext was found. Specify which one to use. Use the '-Context' parameter for PowerShell 
commands and the '--context' parameter for dotnet commands
--search information, some said:Add-Migration MyMigration -context FindPetContext might work,I tried, it did.
--same as the above, for update database, I used Update-Database -context FindPetContext for update the database becasue if i use Update Database,
The same error message shows up. but, anyway, the problem solved, happy.
2330
--test the app, unfortunately, it does not work for the database.
--tried to modify the pet.cs file to apply the default property, still not working.
--tried to initiate with PetsControllerContext, not working;

2021-10-13

19:00
--Continue working on part 4, finally I found out that in the shared/_layout.cshtml, asp-controller for FindPet should be Pets instead of home.
--Now it is working.
--Go back to Pet.cs, modify the property I need in the project, test the app, working.

20:00
--create new records (11 in total) in my database

22:00
--working on the image part
--download images from website without copyright, download three pictures and cross the picture to 300px * 225px;
--insert the pictures to Home page and About page

22:35
--change style of background, fonts, and color, etc

22:00 
--ready to upload to Github and Azure(I actually created a repository at the beginning)
--Hooray




