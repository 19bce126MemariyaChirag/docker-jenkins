  
pipeline{
    agent any
    environment
    {
        NEW_VERSION='1.3.0'
        SERVER_CREDENTIALS=credentials('dockerhub-jenkins')
    }
    stages{
        stage('build'){
            steps{
                echo 'building the application...'
                echo "building the version ...... ${SERVER_CREDENTIALS}"
            } 
        }
        stage('test'){
            steps{
                echo 'testing the application'
            }
        }
        stage('deploy'){
            steps{
                echo 'deploying the applicatin for the demo '
                // withCredentials([usernamePassword(credentials:'dockerhub-jenkins',usernameVariable:USER,passwordVariable:PWD) ]){  
                //     sh "some script   ${USER} ${PWD}"
                // }
                  
            }
        }
    }
}