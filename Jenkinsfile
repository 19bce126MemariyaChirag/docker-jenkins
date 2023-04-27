pipeline{
    agent any
    environment
    {
        NEW_VERSION='1.3.0'
        SERVER_CREDENTIALS=credentials('')
    }
    stages{
        stage('build'){
            steps{
                echo 'building the application...'
                echo "building the version ${NEW_VERSION}"
            } 
        }
        stage('test'){
            steps{
                echo 'testing the application'
            }
        }
        stage('deploy'){
            steps{
                echo 'deploying the applicatin for the demo'
            }
        }
    }
}