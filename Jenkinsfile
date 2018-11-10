pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /root/.m2:/Users/chalkdigital/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh '/Users/chalkdigital/software/apache-maven-3.3.3/bin/mvn -B -DskipTests clean package' 
            }
        }
    }
}
