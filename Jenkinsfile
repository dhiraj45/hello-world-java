pipeline {
    agent any
    
    stages {
        stage('build') {
            steps {
                sh 'python hello_world.py'
                sh 'mkdir ~/Documents/deploy && cp hello_world.py ~/Documents/deploy/hello_world.py' 
            }
        }
    }
}
