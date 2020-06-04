pipeline
{
    agent any
    stages
    {
        stage('Lint HTML') {
			steps {
				sh 'tidy -q -e *.html'
			}
		}
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