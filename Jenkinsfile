pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/KetkiAshtankar/RobotFrameWork.git'
            }
        }
        stage('Install Requirements') {
            steps {
                bat '"C:\Users\HP\AppData\Local\Programs\Python\Python313\python.exe" -m pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                bat '"C:\Users\HP\AppData\Local\Programs\Python\Python313\python.exe" -m robot TestCodes'
            }
        }
    }
}
