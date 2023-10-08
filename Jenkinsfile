Write a Scripted Pipeline to execute the build pipeline with all the 9 goals of Maven.
pipeline {
    agent any
    tools {
        maven 'maven1'
    }
    stages {
        stage('fetch') {
            steps {
                echo 'Fetching the Maven Project from github'
                git branch: 'main',
                url: 'https://github.com/Gauravkumar1502/DevOpsPractical'
            }
        }
        stage('validate') {
            steps {
                echo 'Validating the Maven Project'
                sh 'mvn validate'
            }
        }
        stage('clean') {
            steps {
                echo 'Cleaning the Maven Project'
                sh 'mvn clean'
            }
        }
        stage('compile') {
            steps {
                echo 'Compiling the Maven Project'
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
                echo 'Testing the Maven Project'
                sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                echo 'Packaging the Maven Project'
                sh 'mvn package'
            }
        }
        stage('verify') {
            steps {
                echo 'Verifying the Maven Project'
                sh 'mvn verify'
            }
        }
        stage('install') {
            steps {
                echo 'Installing the Maven Project'
                sh 'mvn install'
            }
        }
    }
}