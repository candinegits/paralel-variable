  Pipeline {
    agent {
      label{
        lablel 'slave1'
      }
    }
    stages {
        stage('git-clone'){
            parallel{
                stage('parallel-1'){
                    steps{
                        sh 'lscpu'
                    }
                }
                stage('parallel-1a'){
                    steps{
                        sh'free -m'
                    }
                }
            }
        }
        stage('systemcheck-stage'){
            parallel{
                stage('parallel-2'){
                    steps{
                        sh'free -g'
                    }
                }
                stage('parallel-2a'){
                  agent {
                     label{
                       lablel 'slave2'
                         steps{
                        sh'lscpu'
                    }
                }
            }
        }
        stage('systemanalysis-stage'){
            parallel{
                stage('parallel-3'){
                    steps{
                        sh 'whoami'
                    }
                }
            }
        }
    }
} 
