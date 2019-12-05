pipeline {
    agent {
        docker {
            image 'maven'
            args '-v /home/ds/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B clean package'
            }
        }
    }
}