pipeline{
    agent any
    tool{
        maven '$maven-name'
    }
    stages{
        stage( 'git-clone'){
            steps{
                sh 'lscpu'
            }
        }
        stage( 'system check'){
            steps{
                sh 'whoami'
            }
        }
    }
}
