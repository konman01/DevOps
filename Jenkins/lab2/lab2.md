## Click on New Item , give lab1-pipeline as Project Name, Select Pipeline in the list and click okay

![Screenshot 2023-02-19 at 5 57 00 AM](https://user-images.githubusercontent.com/33331778/219946800-85bbb48c-4199-490f-a660-b45501d2107b.png)

## Paste the following script in the pipeline script and save

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

![lab2-2](https://user-images.githubusercontent.com/33331778/219947018-9390ed81-8730-40ca-b06a-e5483cb21185.png)

## click on the build

![lab2-3](https://user-images.githubusercontent.com/33331778/219947208-406b99a1-ba64-4eeb-9755-a495dafe6a1b.png)

![lab2-4](https://user-images.githubusercontent.com/33331778/219947266-b94dbe04-a5b3-493b-bb7d-8e911b78b1d2.png)

