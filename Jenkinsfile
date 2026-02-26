pipeline {
    agent {
        label 's1'
    }

    stages {
        stage('Build java project and deploy ') {
            steps {
               git 'https://github.com/Sharath-yp25/java.git'
               sh '''javac Test.java
                    java Test'''
            }
        }
         stage('Build maven project and deploying ') {
            steps {
              git 'https://github.com/Sharath-yp25/mavenproject.git'
              sh 'mvn package'
            }
        }
    }
}
