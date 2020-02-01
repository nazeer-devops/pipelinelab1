pipeline{
    agent any
    
    stages {
        stage('stage checout'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GIT_CREDENTIALS', url: 'https://github.com/nazeer-devops/Secondexcercise.git']]])
            }
        }
        stage('stage output'){
            steps{
                sh label: '', script: 'ls -al'
            }
        }
    }
}
