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
                parallel(
                    "TaskOne":{
                        echo "task one stuff part 1"
                        echo "task one stuff part 2"
                        echo "task one stuff part 3"
                    },
                    "TaskTwo":{
                        echo "task two stuff part 1"
                        echo "task two stuff part 2"
                        echo "task two stuff part 3"
                    }
                )
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
