pipeline {
            agent any

stages {
        stage ('Compile Stage'){

            steps{
                withMaven(maven : 'maven_3_5_0'){
                sh 'mv clean compile'
                }
            }
        }


        stage ('Testing Stage'){

            steps{
                withMaven(maven : 'maven_3_5_0'){
                sh 'mv Test'
                }
            }
        }


        stage ('Deployment Stage'){

            steps{
                withMaven(maven : 'maven_3_5_0'){
                sh 'mv deploy'
                }
            }
        }
        }
}
