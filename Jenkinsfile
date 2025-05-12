pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mkdir -p out'
                sh 'javac -d out HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java -cp out HelloWorld'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Simulating deployment..."'
                sh 'cp out/HelloWorld.class /tmp/'  // change path as needed
            }
        }
    }
}
