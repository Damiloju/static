pipeline{
    agent any
    stages{
        stage("Upload To AWS"){
            withAWS(credentials:'aws-statci',region:'eu-west-1') {
                s3Upload(file:'index.html', bucket:'static-udacity-dam', path:'index.html')
            }
        }
    }
    
}