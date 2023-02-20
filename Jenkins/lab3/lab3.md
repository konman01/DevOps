# Build by pulling Jenkinsfile in github

## Jenkinsfile in Github
1. Create Jenkins file in lab3 folder and paste the following script
```
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
```
2. Check-in the script to github

![lab3-6](https://user-images.githubusercontent.com/33331778/220000626-ab176645-b1da-42ad-99d5-54f43ca410a0.png)

## Create new Item

1. Click on New Item 
2. Give lab1-pipeline as Project Name
3. Select Pipeline in the list and click okay

![lab3-1](https://user-images.githubusercontent.com/33331778/219998100-8b585f37-5ed0-4139-9783-187d45578fe0.png)

## Define SCM for Pipeline Sciprt

1. From the Definition field, choose the Pipeline script from SCM option.
2. From the SCM field, choose the type of source control system of the repository containing your Jenkinsfile.
3. Give the git repository url where Jenkinsfile is created
4. As the Jenkinsfile is in the lab3 folder, define the path to the folder in Script Path

![lab3-7](https://user-images.githubusercontent.com/33331778/220001044-ddf0a766-a96b-4179-9f05-d24885780efb.png)

## Build

1. Go to the pipe line created
2. Click on Build
3. Click on console to check the logs

![lab3-4](https://user-images.githubusercontent.com/33331778/219999084-9563e178-0c8f-43d6-b6c1-04a28a003ba1.png)
![lab3-5](https://user-images.githubusercontent.com/33331778/219999089-d6f2938d-523c-46d5-8ed9-080b917d0831.png)




