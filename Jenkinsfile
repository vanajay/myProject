pipeline {
agent any

      stages{
         stage('CheckOut'){
          steps{
            git 'https://github.com/vanajay/myProject.git'
            }
         }

         stage('Build'){
           steps{
             sh 'mvn clean compile'
           }
         }

         stage('Test'){
           steps{
              sh 'mvn test'
              junit  '**/target/surefire-reports/TEST-*.xml'
           }
         }
      }

}
