pipeline {
    agent any  // تعني أن جيكنز ينفذ الـ Pipeline في أي جهاز

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                powershell 'mvn clean install'  // استخدم powershell بدلاً من sh
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                powershell 'mvn test'  // استخدم powershell بدلاً من sh
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                powershell 'mvn deploy'  // استخدم powershell بدلاً من sh
            }
        }
    }
}
