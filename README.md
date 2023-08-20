# Cat-Dog-Classification

## How to Run

1. conda create -n catdog python=3.7 -y
2. conda activate catdog
3. pip install -r requirements.txt
4. python main.py
5. open in browser: http://localhost:8080/



# GCP points to take care of
    1. Application name should be main.py
    2. in main.py host should be '127.0.0.1' instead of '0.0.0.0' of AWS
    3. app.yaml contains deployment as well as run configuration
    

# GCP Deployment



## 1. Login to gcp console.

## 2. Download gcloud sdk : 
     - https://dl.google.com/dl/cloudsdk/channels/rapid/GoogleCloudSDKInstaller.exe

## 3. Create a new project in GCP
      select the newly created project

## 4. Use app engine service

## 5. run command "gcloud init" in installed sdk terminal
	- configure with your current project settings
   ## a. Pick configuration to use:
        [1] Re-initialize this configuration [default] with new settings
        [2] Create a new configuratiom
        Please enter your numeric choice:  2
	
   ## b. Choose the account you would like to use to perform operations for this configuration:
       [1] ravi0dubey@gmail.com
       [2] Log in with a new account
           Please enter your numeric choice:  1
	   
   ## c. Pick cloud project to use:
       [1] annular-splice-382510
       [2] dog-cat-project-382511
       [3] youtube-analysis-ravi
       [4] Enter a project ID
       [5] Create a new project
       
       Please enter numeric choice or text value (must exactly match list item):  2
       Your current project has been set to: [dog-cat-project-382511].

## 6. In the command prompt or gitbash terminal 
      Ensure we are in correct directory where our project reside

## 7. run command in command prompt or gitbash terminal "gcloud app deploy"
     - select region 18 for us-east-1
     - Do you want to continue - 'Y'
	
## 8. To view your application in the web browser run:
      $ gcloud app browse

	
	
	
