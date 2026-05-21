pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Build – Compile and package the code using Maven .'
            }
        }
        stage('Unit & Integration Tests') {
            steps {
                echo 'Unit and Integration Tests – Run unit tests with JUnit and integration tests with Postman.'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Code Analysis – Analyse code quality and standards using SonarQube ).'
            }
        }
        stage('Security Scan') {
            steps {
                echo ' Scan for vulnerabilities using OWASP Dependency-Check or Snyk.'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo ' Deploy to Staging – Deploy artifact to an AWS EC2 staging server using Ansible/SSH.'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Integration Tests on Staging – Run end-to-end tests on staging with Selenium.'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploy to Production – Promote build to production EC2 instance using AWS.'
            }
        }
    }
}
