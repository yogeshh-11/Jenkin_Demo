pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yogeshh-11/Jenkin_Demo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'javac HelloWorld.java'
            }
        }
        stage('Run') {
            steps {
                echo 'Running...'
                bat 'java HelloWorld'
            }
        }
    }
}
