pipeline {
    agent any
    stages {
        stage('git-clone'){
            paralel{
                stage('paralel-1'){
                    steps{
                        sh 'lscpu'
                    }
                }
                stage('paralel-1a'){
                    steps {
                        sh'free -m'
                    }
                }
            }
        }
        stage('systemcheck-stage'){
            paralel{
                stage('paralel-2'){
                    steps {
                        sh'free -g'
                    }
                }
                stage('paralel-2a'){
                    steps {
                        sh'lscpu'
                    }
                }
            }
        }
    }
}
