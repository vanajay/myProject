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
      }

}
