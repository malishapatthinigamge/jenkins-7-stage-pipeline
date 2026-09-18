pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1 - Build: Compile and package the code'
                echo 'Tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2 - Run unit tests to check code works, and integration tests to check components work together'
                echo 'Tools: JUnit (unit tests), Selenium (integration tests)'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Stage 3 - Analyse the code to make sure it meets industry standards'
                echo 'Tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Stage 4 - Scan the code and dependencies for security vulnerabilities'
                echo 'Tool: OWASP Dependency-Check (or Snyk)'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5 - Deploy the application to a staging server'
                echo 'Tool: AWS CLI / AWS CodeDeploy to an AWS EC2 staging instance'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6 - Run integration tests on staging (production-like environment)'
                echo 'Tools: Selenium, Postman/Newman'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7 - Deploy the application to the production server'
                echo 'Tool: AWS CodeDeploy to an AWS EC2 production instance'
            }
        }
    }
}
