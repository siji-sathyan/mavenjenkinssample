pipeline{
    agent any
    stages{
        stage('Initial'){
            steps{
            withMaven(maven : 'maven_3_8_2'){
            
                sh 'mvn clean'
                }
            }
        }
    stage('Compile'){
            steps{
            withMaven(maven : 'maven_3_8_2'){
                sh 'mvn compile'
                }
            }
        }
    stage('Package'){
            steps{
            withMaven(maven : 'maven_3_8_2'){
                sh 'mvn package'
                }
            }
    stage('Deploy'){
            steps{
            withMaven(maven : 'maven_3_8_2'){
                sh 'mvn deploy'
                }
            }
        }
    }
    
}

