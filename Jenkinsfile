pipeline {
    agent any
    environment {
        python3 = "C:\\Users\\Student\\AppData\\Local\\Programs\\Python\\Python313\\python.exe"
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building python script'
                bat "${python3} code.py"
                echo 'Finnishing python script'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
