pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/your-username/kafka-project.git'
            }
        }
        stage('Run Kafka Producer') {
            steps {
                sh 'python3 producer.py'
            }
        }
        stage('Run Kafka Consumer') {
            steps {
                sh 'python3 consumer.py'
            }
        }
    }
}
