# SampleApp_Mac
template for creating a MacOS app from a JAR file

<b>How to use:</b>

  1) Download the directory(duh)
  
  2) right-click "App.app" (might display as simply "App") and select "show package contents"
  
  3) go to Contents > Resources and replace "application.icns" with the desired app icon (and name it "application.icns")
    
    3a. if for whatever reason you don't want your icon to be called application.icns, go to Info.plist
    and under "<key>CFBundleIconFile</key>", where it says "<string>application.icns</string>", change "application.icns" to "<yourIconFile.icns>"
    
  4) go to Contents > MacOS and replace "SampleApp.jar" with the .jar file of your app
  
  5) open "launcher" with any text editor
  
    5a. under "# Constants" replace APP_JAR="SampleApp.jar" with APP_JAR="<yourFile.jar>"
  
    5b. in the next line, replace APP_NAME="Sample" with APP_NAME="<yourAppName>"
    
  6) now, "App.app" (you should rename it now, if you haven't already) should display your app icon and run your .jar file when clicked on
  
  
