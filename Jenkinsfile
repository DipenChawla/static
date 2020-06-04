pipeline
{
    agent any
    stages
    {
        stage("Upload AWS")
        {
            steps{
                withAWS(region: 'eu-west-1', credentials:'aws-static') {
                s3Upload(file:'index.html', bucket:'udacity-cicd-static', path:'index.html')
                }
            }
        }
    }
}