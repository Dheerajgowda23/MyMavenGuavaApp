pipeline {

    agent any

    stages {

        stage('Build') {

            steps {

                sh 'mvn clean compile'

            }
        }

        stage('Test') {

            steps {

                sh 'mvn test'

            }
        }

        stage('Package') {

            steps {

                sh 'mvn package'

            }
        }

        stage('Run') {

            steps {

                sh 'mvn exec:java -Dexec.mainClass="com.example.App"'

            }
        }
    }
}
