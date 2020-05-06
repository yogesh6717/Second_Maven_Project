  
  
pipeline {
    agent any
 environment {
    PATH = "/Program Files/apache-maven-3.3.3/bin:$PATH"
  }
    stages {
        stage("Git Checkout") {
            steps {
                git credentialsId: 'b8797411-cbfd-4ba2-92f4-9d1dd54117e3', url: 'https://github.com/yogesh6717/Second_Maven_Project'
            }
        }
        stage("Maven Build") {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
