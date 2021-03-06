# Run a demo SubethaSMTP Server #

Download the most recent jar with depandancies file from the releases section on Github and run the command...
```
java -cp subethasmtp-j3.1.8-jar-with-dependencies.jar org.subethamail.examples.BasicSMTPServer
```

...where `subethasmtp-j3.1.8-jar-with-dependencies.jar` is the release file you downloaded.  

To test, use `TELNET` or an SMTP client to connect to the now-running server on TCP port 25000.

# Enable logging #

Note that SubethaSMTP uses the SLF4J logging framework. When the program starts up, it will look for a compatible logging connector in the classpath. If none is found it will print a warning message to the console and then silently toss any log messages generated by the program.   

If you want to see the logging messages, you need a compatible connector in the classpath. 

You can download connectors from the [SLF4J website](http://www.slf4j.org/download.html). The `Simple` connector is very simple and just prints log messages to stderr.  Note that the version of the connector must match the version that SubethaSMTP was built against. 
  

# Editing in Eclipse

1. Clone the repository from GitHub to your local machine. 
2. Open Eclipse and do `Import->Maven->Existing Maven Projects`
3. Right click on the `POM.XML` file and select `Run As->Maven Install`

