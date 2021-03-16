pipeline {
    agent any 
    stages {
        stage('Checkout') { 
            steps {
            sh "rm -rf MavenJenkins"
            sh "git clone https://github.com/jibraniqbal2018/MavenJenkins.git"

            }
        }
        stage('Clean') { 
            steps {
            sh "mvn clean -f MavenJenkins"

            }
        }
        stage('Deploy') { 
            steps {
            sh "mvn package -f MavenJenkins"
                
            }
        }
    }
}
