pipeline{
    agent any
    stages{
        stage('parallel-level'){
            paralel{
                stage('subjob-1'){
                    steps{
                        sh 'lscpu'
                    }
                }
                stage('subjob-2'){
                    steps {
                        sh'free -m'
                    }
                }
            }
        }
        stage('systemcheck-stage'){
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
