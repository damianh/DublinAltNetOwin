Dublin Alt.Net Owin and Katana
=========

This repository contains the source code used in the presentation. Disclaimer: it is not an example of a well architected application, but rather demonstrates some of the key areas in building an OWIN compliant application.

There are 4 projects:

  - KatanaConsoleApplication1.csproj and KatanaWebApplications1.csproj are examples of the project templates installed when you install the [Katana.vsix] visual studio extension. They demonstrate the minimum required to run an owin application self-hosted (HttpListener) or on asp.net (SystemWeb)
 
  - PackageExamples.csproj demonstrates various Owin.* and Microsoft.Owin.* packages in various Startup configurations. Also contains some sample tests

  - NancySignalrRaven.csproj is an example application that combines.. Nancy, SignalrR and RavenDB as well as various middleware and dependency injection.
Dillinger is a cloud-enabled HTML5 Markdown editor.

Using NancySignalrRaven App
-

 1. Set NancySignalrRaven as startup project and hit F5. Use Chrome Dev tools / FireBug to view the traffic.
 2. Browse to http://localhost:2020 to see the root katana test page as served by Microsoft.Owin.Diagnostics
 3. http://localhost:2020/fault to see what happens when an exception occurs and we've enabled showing of exceptions (via Microsoft.Owin.Diagnostics)
 4. http://localhost:2020/files to browse your C:\ drive which is protect by Basic Auth (Microsoft.Owin.Auth.Basic). Type in any username, and 'damo' for password.
 5. http://localhost/site/ to see the chat home page. Open a couple of chat windows, broadcast some messages and then browse the logs.

License
-

MIT

Questions, criticisms, compliments or otherwise, [@randompunter]

Have fun!

  [katana.vsix]: http://katanaproject.codeplex.com/releases/view/102220
  [@randompunter]: http://twitter.com/randompunter
  