# jsp_internationalization
jsp_internationalization
Internationalization is the process by which I can make my web application to use all languages.
In case of a basic JSP/Servlet webapplication, the basic approach would be using JSTL fmt taglib in combination with resource bundles. Resource bundles contain key-value pairs where the key is a constant which is the same for all languages and the value differs per language. Resource bundles are usually properties files which are loaded by ResourceBundle API.

Here's an example how to internationalize the login form of your webapplication with properties file based resource bundles.

Create the following files and put them in some package, e.g. com.example.i18n (in case of Maven, put them in the package structure inside src/main/resources).

text.properties (contains key-value pairs in the default language, usually English)

 login.label.username = Username
 login.label.password = Password
 login.button.submit = Sign in
 
text_nl_NL.properties (contains Dutch (nl) key-value pairs)

 login.label.username = Gebruikersnaam
 login.label.password = Wachtwoord
 login.button.submit = Inloggen
 
text_es_AR.properties (contains Spanish (es) key-value pairs)

 login.label.username = Nombre de usuario
 login.label.password = Contraseña
 login.button.submit = Acceder
 
 Resource files are named as per locale code. Pdf file for localecodes is also attached with this project

