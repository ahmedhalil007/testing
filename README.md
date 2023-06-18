# Testing_lab

# Goal:
Testing for smoke and regression on the Mocca Commerce site ```https://moccacommerce.com/``` 

Project is based on using Selenium and Java 

# Set up

## Setup Visual Studio Code For Java
- Install Java Extension Pack and create Java project in Visual Studio Code.
- For the Java project, select no build tools and write the name of the project.
- The new project will open in a new window of Visual Studio Code and contain a java file, lib and src folders, and a readme file.

## Setup Selenium WebDriver

-Download selenium web driver for java, it will be zip file (e.g. selenium-java-4.7.2.zip).
```https://www.selenium.dev/downloads/```
- There will be several jar files after unzipping the file. It's crucial to include EVERY single jar file in the project's dependencies.
  •The client-combined-4.7.2.jar is required for the compilation of our        Selenium code, 
  •The remaining jars are required for executing Selenium.
- By selecting "+" next to Referenced Libraries, all jars can be added to the project.

## Setting up SafariDriver

Safari driver is used in this project. If you use Mac OS X, to set up the Safari Driver, you need to do the following:
Safari driver is used in this project. If you use Mac OS X, in order to set up the Safari Driver, you need to do the following:
1.	 open the Safari browser and click on "Safari" in the upper left corner
2.	then click on ```Preferences```
3.	then click on ```Show Develop menu in menu bar```
4.	then click on ```Develop``` in the menu bar and allow remote automation.

Then, in test code you need to use “WebDriver driver = new SafariDriver();”





## Setting up ChromeDriver 

-	Download ChromeDriver. The ChromeDriver major version has to match your Chrome version.
-	Unzip ChromeDriver zip and move it to a central folder that will be referenced by multiple projects (e.g. ~/dev/selenium/bin/ on a Mac)
-	Configure ChromeDriver to be discoverable by WebDriver in one of two ways:
-	Option1 – add ChromeDriver binary to the PATH variable
           export PATH=$PATH:~/dev/selenium/bin/ (Mac)
 Test that it’s set correctly by executing “chromedriver” from another directory – you should see ChromeDriver start and you can press CTRL-C to stop it; this will allow multiple projects to use the same ChromeDriver binary.
-	Option 2 – add the path to ChromeDriver in your test code:
•	System.setProperty(“webdriver.chrome.driver”, “~/dev/selenium/bin/chromedriver”);
Then, in test code you need to use “WebDriver driver = new ChromeDriver();”


# Run Selenium

Now that all the setup is in place, we’re ready to develop and run Selenium code.
After we create the Selenium script and make sure that we entered all information correctly, we can run Java project from Java Projects view. In the upper right corner of VS code we will find a play button that will run the code.








