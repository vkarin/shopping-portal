pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build'){
            steps{
                sh 'npm install'
              }
        }
        stage('test'){
            steps{
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                sh 'npm run package'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline for shoppin-portal application has completed...'
        }
        
    }
    
}
