pipeline{
    agent any
    stage('build'){
        steps{
            sh 'npm install'
        }
    }
    stage('deploy'){
        steps{
            nodejs(nodeJSInstallationName: 'nodejs') {
                withAWS(credentials: 'aws-credentials') {
                    sh 'serverless deploy'
        }
    }


}