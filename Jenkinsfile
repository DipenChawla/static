pipeline
{
    agent any
    stages
    {
        stage("Upload AWS")
        {
            steps{
                withAWS(credentials:'aws-static') {
                    s3Upload(file:'index.html', bucket:'udacity-cicd-static', path:'index.html')
                }
            }
        }
    }
}