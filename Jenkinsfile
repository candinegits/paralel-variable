pipeline{
    agent any
    stages{
        stage('parallel-level'){
            parallel{
                stage('subjob-1'){
                    steps{
                        echo 'lscpu'
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
    }
}
           
