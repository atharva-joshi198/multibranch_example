
pipeline{
    agent any
    stages{
        stage('checkour')
        {
            steps{
                git branch: 'side', credentialsId: '6f65092d-55a4-4024-93e0-13473e4bd722', url: 'https://github.com/atharva-joshi198/jenkins_example.git'
            }
        }
        stage ('build')
        {
            steps
            {
                bat 'Build.bat'
            }
        }
        stage ('Compile')
        {
            steps
            {
                 bat 'Compile.bat'
            }
        }
        stage('test')
        {
            steps
            {
                 bat 'Test.bat'
            }
        }
        stage ('Deploy')
        {
            steps
            {
                bat 'Deploy.bat'
            }
        }
        
    }
}
