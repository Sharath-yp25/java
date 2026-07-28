pipeline {
    agent any

    stages {
        stage('Cloning java github repository') {
            steps {
                git 'https://github.com/Sharath-yp25/java.git'
            }
        }
        
        stage('Compile and execute java project') {
            steps {
               bat '''javac Test.java
                      java Test'''
            }
        }
        
         stage('Cloning maven github repository') {
            steps {
                git 'https://github.com/Sharath-yp25/mavenproject.git'
            }
        }
        
         stage('Generating package for maven') {
            steps {
              bat 'mvn package'
            }
        }
    }
}
