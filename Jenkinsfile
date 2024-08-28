pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
       
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running Unit and Integration Tests...'
            
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Performing Code Analysis...'
           
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Performing Security Scan...'
         
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to Staging...'
            
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running Integration Tests on Staging...'
        
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to Production...'
       
            }
        }
    }
    post {
        always {
            echo 'Sending notification emails...'
            mail to: 'IrfanBoenardi1@gmail.com',
                 subject: "Jenkins Pipeline ${currentBuild.IrfanBoenardi}",
                 body: "The build ${currentBuild.IrfanBoenardi} has finished with status: ${currentBuild.result}. Check console output at ${env.BUILD_URL} to view the results."
        }
    }
}
