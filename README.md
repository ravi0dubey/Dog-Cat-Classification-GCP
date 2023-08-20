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

## 2. Create a new project in GCP
   ![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/3b9fe61e-c0a8-43c6-a76b-4f89ab75d6b1)
   
   -Select the newly created project

## 3. Use app engine service
   ![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/a7080f9f-c285-48c9-9358-9b40e9cccc2a)

## 4. Download gcloud sdk : 
     - https://dl.google.com/dl/cloudsdk/channels/rapid/GoogleCloudSDKInstaller.exe
## 5. run command "gcloud init" in installed sdk terminal
	- configure with your current project settings
   ## a. Pick configuration to use:
        [1] Re-initialize this configuration [default] with new settings
        [2] Create a new configuratiom
	[3] switch to and re-initialize existing configuration
        Please enter your numeric choice:  2
   ## b. Enter configuration name:
   	Enter value "dog-cat-project"
   ## c. Choose the account you would like to use to perform operations for this configuration:
       [1] ravi0dubey@gmail.com
       [2] Log in with a new account
       
           Please enter your numeric choice:  1
	   
   ## d. Pick cloud project to use:
       [1] annular-splice-382510
       [2] dog-cat-project-396516
       [3] youtube-analysis-ravi
       [4] Enter a project ID
       [5] Create a new project
       
       Please enter numeric choice or text value (must exactly match list item):  2
       Your current project has been set to: [dog-cat-project-396516].

![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/e1f84ff1-2b51-4761-879b-9cabdfe8e5d2)
![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/a8540e2c-bbc7-41a5-9e77-a41b69d10053)


## 6. In the command prompt or gitbash terminal 
      Ensure we are in correct directory where our project reside

## 7. run command in command prompt or gitbash terminal "gcloud app deploy"
     - select region 18 for us-east-1
     - Do you want to continue - 'Y'
![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/f078a49d-32b4-4fdc-b076-ff6a64f30cef)

     - post deployment
![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/ab6b2df4-b9a3-4a62-91be-c6d2d9a4c819)


## 8. To view your application in the web browser run command in the powershell:
      - "gcloud app browse"
![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/02ea7844-de75-4c7a-94b2-0704e358ef18)


## 9. Click on the URL to do the Prediction
![image](https://github.com/ravi0dubey/Dog-Cat-Classification-GCP/assets/38419795/c5385a36-e8b6-446a-b0f8-db90b676d311)

  
	
	
