pipeline{
    agent any
    stages{
        stage("Upload To AWS"){
            withAWS(credentials:'aws-static',region:'us-west-2') {
                s3Upload(file:'index.html', bucket:'static-udacity-dam', path:'index.html')
            }
        }
    }
    
}