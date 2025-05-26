pipeline {
    agent any

    stages {

        stage('getEnv'){
            steps {
                sh 'printenv'
            }
            
        }

        stage("Build"){
            steps {
                sh "./mvnw install"
                sh "ls -lrt target/*.jar"
            }
        }
    }
}