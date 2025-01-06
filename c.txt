sudo apt install docker.io

sudo docker pull jenkins/jenkinssudo 
docker run -p 8080:8080 -p 5000:5000  -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts




<!DOCTYPE html> 
<html> 
<head> 
<title>Welcome Page</title> 
</head> 
<body> 
<h1>Welcome to Cloud Computing</h1> 
</body> 
</html> 

sudo apt update 
sudo apt install apache2 -y 
sudo systemctl start apache2 
sudo systemctl enable apache2 

----------------------------------------

dism /online /enable-feature /featurename:IIS-WebServer /all
net start w3svc
cd C:\inetpub\wwwroot 

-----------------------------------------

instance vpc
	 public subnet
	 enable

chmod 400 private
ssh -i "private.pem" 172.20.2.215

-----------------------------------------

labda additional confi >> function url > auth none

https://<your-function-url>?course=hpcsa 

-------------------------------------------

def lambda_handler(event, context):
    # Retrieve the 'course' parameter from the query string
    course = event.get('queryStringParameters', {}).get('course', '').lower()
    
    # Prepare a response message based on the course
    if course == 'hpcsa':
        message = "Welcome to HPCSA course"
    elif course == 'ditiss':
        message = "Welcome to DITISS course"
    elif course == 'dbda':
        message = "Welcome to DBDA course"
    else:
        message = "Course not found. Please choose from 'hpcsa', 'ditiss', or 'dbda'."
    
    # Return the response
    return {
        'statusCode': 200,
        'body': message
    }



