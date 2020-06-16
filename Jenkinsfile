pipeline {
agent any
     tools{
       Maven 'M3'
     }

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
