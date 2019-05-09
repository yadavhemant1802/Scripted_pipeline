pipeline{
    agent any
    stages{
        stage('Git-checkout'){
            steps{
                echo "copy code from git hub";
                git credentialsId: '68e5a7f4-f554-4021-b6d3-d481aeacda1f', url: 'https://github.com/yadavhemant1802/Scripted_pipeline.git'
            }
            
        }
        stage('compile'){
            steps{
                echo "This will compile code"
                bat label: '', script: 'Compile.bat'
            }
        }
        stage('build'){
            steps{
                echo "Build this code";
                bat label: '', script: 'Build.bat'
            }
        }
        
        stage('deploy'){
            steps{
                echo "Build this code";
                bat label: '', script: 'Deploy.bat'
            }
        }
        
        }
    }
