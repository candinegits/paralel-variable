pipeline{
    agent any
    }
    stages{
        stage( 'git-clone'){
            steps{
                checkout'checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Git', url: 'https://github.com/candinegits/paralel-variable.git']]]) '
            }
        }
        stage( 'system check'){
            steps{
                sh 'whoami'
            }
        }
    }
