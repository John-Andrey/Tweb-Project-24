# Tweb-Project-24



###



###

<h1 align="center">Hey there 👋</h1>

###

<h3 align="left">👩‍💻  The Web Technologies Project</h3>

###

<p align="left">Project requirements<br>The exam project consists of a web application consisting of<br><br>a server-side application created with JakartaEE (therefore, based on Servlet), connected to a SQL database, which sends and receives data in JSON format.<br>a client-side application that will be specified after the corresponding part of the course has been covered.<br>The application can concern any theme and you can choose whether to create an application in which the business logic is managed mostly by the server, mostly by the client, or equally distributed between the two. In general, keep in mind that:<br><br>if the application is particularly oriented towards interactivity and graphics (think for example of a video game with important graphics) there will be significant client-side processing<br>if the application is particularly data-oriented, and processes sensitive (or otherwise non-public) data to provide the user with the results of such processing, without the user having access to the data itself, there will be significant server-side processing; think of the logic of a board game: the server must impose the rules, or the clients would try to cheat!<br> an application could easily have both characteristics<br> In general, the disadvantage of server-side processing is that the server, which is supposed to receive many requests, can become overloaded. The disadvantage of client-side processing is that the client must have the necessary data in its possession, and this is not always possible or effective.<br><br> The application will have to manage login/logout at least in the simplified way seen in class; if you want to offer a more serious, more secure login/logout based on your Google account, you can do so, but it is not mandatory.<br><br> Server-Side Application Minimum Requirements<br> Java language specification &gt;= 8, Java 11 and SDK 21 are suggested<br> At least two different Servlets in addition to the one you have takes care of the Login. Be careful to divide the tasks sensibly between the three!<br> Using the Gson library for receiving and sending data<br> Use of connection pooling in the DB<br> At least 6 tables in the database<br> Plan for at least 2 test users, each with a reasonable amount of data to try out the application. Of course, depending on the type of application, you may need more users (if you implement the Bridge game you will need at least 4...)<br> Plan for at least 1 user with "superpowers": a manager, a superuser, an administrator... the point is that he must be able to do something that other users cannot do (for example, in an eCommerce the manager might want to insert new products from sell, which normal users usually cannot do).<br> Error handling<br> Simplified error handling is sufficient, but it allows you to effectively debug the application (not all the examples we have seen in class had this feature: for example, leaving the catch block of an exception empty is a perfect way to complicate debugging! it's fine just for examples and small exercises...). Some suggestions:<br><br> use 404 Not Found when it is clear from the first path checks that a non-existing resource has been requested<br> in case of internal exceptions (typically: SQL exception) use 500 Internal Server Error, but take care to at least print the stack trace of the exception to the console (exception.printStackTrace( ))<br> use 401 Not Authorized if a request arrives for which the current user is not authorized or which requires a login that has not been logged in<br> Evaluation criteria<br> A server-side app that does not respond correctly to client-side app requests, or that does not comply with the minimum requirements, will not be considered valid for discussion of the project. The "positive" evaluation elements will be the following:<br><br> organization clear route (http METHOD + path) with respect to the operations that the server-side app allows you to request<br> good organization of the code, i.e. logical division of tasks between the different servlets and the different classes<br> good management of database connections, including the use of transactions with rollback and commit if necessary<br> The important thing with respect to these characteristics is that your choices are thoughtful and reasonably effective with respect to the type of application you are thinking of creating; there is no "optimal" choice, usually you have to evaluate some tradeoff (and the time needed to implement a solution, especially if it is an application for examination and not a commercial project, is an element of evaluation to be consider among others!).<br><br> Minimum Client-Side Application Requirements<br> must be written with the Typescript language<br> the view must be created in HTML + CSS; it is not forbidden (if you know them) use default CSS (e.g. Bootstrap) or preprocessors like SASS or SCSS.<br> must use an MVVM framework with the following alternatives:<br> for those without prior knowledge, the use of React in combination with Vite is recommended (as seen in class)<br> for those who already know it or are very keen to learn it, it is possible to use Angular instead<br> it is also possible for the same reasons to use React in combination with some other framework (e.g. Next.js) but this solution complicates things quite a bit so it is only recommended if you are already familiar with it<br> you can use third-party packages but NOT already made UI components: you have to build them yourself using the framework you have chosen (or better: if you use third-party UI components they will not be counted in the 8 mentioned below)<br> must interact with the backend (exploiting most of the routes provided by the backend<br> it must be a single-page application with at least 8 components (micro-sub-components do not count such as the items of a list or the rows of a table)<br> must include at least two forms with consequent POST (or PUT, if you have any) requests to the server<br> must include at least one case of communication between sister components via the parent component (i.e.: the user interacts with a component on the screen, and something changes in another component that is neither an ancestor nor a descendant of the first)<br> must allow you to log in to connect both as a "normal user" and as a "special user" (see the instructions for the back-end); the special user will have to have some more interaction possibilities than the normal user<br> Error handling<br> Even in this case, simplified error handling is sufficient. It can be assumed that requests to the back end are well formulated. Depending on the application, it will be possible that a non-existent resource is requested from the back-end due to an entered data by the user; remember in this case that from the point of view of the fetch API a "404 not found" response is a valid response, and this case can be handled by associating appropriate behavior with fetch via then.<br><br> For simplification, you are not required to handle 500 Internal Server Errors on the client side (assuming that, if they occur, it is because there is a bug either in the front-end or in the back-end!).<br><br> Regarding data entry errors by users, you can display an overlaid error message, using as an example the ErrorMsg component present in the "final" version of the RpgPC application.<br><br> Evaluation criteria<br> A client-side app that generates exceptions/errors in the expected interactions with users, or that does not comply with the minimum requirements, will not be considered valid for project discussion. The "positive" evaluation elements will be the following:<br><br> clear organization and understandable component hierarchy<br> effective use of event binding (for UI interaction) and property-binding (to show the effects of state changes)<br> in general, effective use of the tools offered by the framework used<br> As with the back-end, the important thing with respect to these characteristics is that your choices are thoughtful and reasonably effective with respect to the type of application you are thinking of creating, always with the appropriate tradeoffs.</p>

###

<h3 align="left">🛠 Language and tools</h3>

###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="40" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="40" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="40" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tomcat/tomcat-original.svg" height="40" alt="tomcat logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" height="40" alt="java logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" height="40" alt="postgresql logo"  />
</div>

###

<h3 align="left"></h3>

###

<p><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=john-andrey&show_icons=true&locale=en&layout=compact" alt="john-andrey" /></p>

