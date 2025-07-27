pipeline {
   agent any
   stages {
        stage('SCM') {
            steps {
              git url : 'https://github.com/SI-AB-OPGI/Jenkins_Terraform.git' , branch : master
              }
           }
        stage('terraform init') {
            steps { 
               sh 'terraform init'
              }
            }
        stage('terraform validate') {
            steps {
               sh 'terraform validate'
              }
            }
        stage('terraform plan') {
            steps {
               sh 'terraform plan'
              }
            }
        stage('terraform apply') {
            steps {
               sh 'terraform apply'
              }
            }
}
}

         
      
