pipeline
{
    agent any
    stages
    {
        stage("Build")
        {
            steps{
                sh "echo 'Hello Word'"
                sh '''
                echo "Multiple Lines do work?
                echo "They do!!!"
                '''
            }
        }
    }
}