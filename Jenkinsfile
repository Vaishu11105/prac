pipeline{
    agent any
    
    stages{
        stage('git clone'){
            steps{
                 git url: 'https://github.com/Vaishu11105/prac.git',branch: 'main'
            }
           
        }
        stage('build')
        {
            steps{
                bat 'docker compose build'
            }
            
        }
        stage('run')
        {
            steps{
                bat 'docker compose up -d'
            }
        }
    }
}