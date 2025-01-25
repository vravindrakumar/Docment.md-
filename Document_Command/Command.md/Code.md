<powershell>
#Install IIS

Install-WindowsFeature -Name Web-Server -IncludeManagementTools

#Start the IIS service 
Start-Service -NameW3SVC

#Set up a basis HTML page to test the web server
$webpagePath = "C:/intepub/wwwroot/index.html"
@"
<!DOCTYPE html>
<html>
<head>
    <title>My Windows Web Server>/title>
</head>
<body>
      <title>My Windows Web Server demo</title>
</head>
<body>
  <h1>Welcome to My Web server!</h1>
  <p> This is a test served by Internet Informations Services (IIS) on windows Server EC2 instance.
  </p>
  </body>
  </html>
  "@| Out-File-File Path $webpagePath
  
# Restart the IIS service to apply changes

Restart-Service -NameW3SVC
</powershell>
  