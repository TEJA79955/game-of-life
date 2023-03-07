pipeline {
    agent {label 'JDK_8'}
    stages {
        stage('vcs') {
            steps {
                git url: 'https://github.com/khajadevopsmarch23/game-of-life.git',
                    branch: 'don'
            }
        }
        stage('package') {
            steps {
                sh """
                     export PATH=/usr/lib/jvm/java-8-openjdk-amd64/bin:$PATH 
                     mvn package
                   """
            }
        }
    }
}        
