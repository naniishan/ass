pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: false, description: '', name: 'java')
        booleanParam(defaultValue: false, description: '', name: 'nginx')
        booleanParam(defaultValue: false, description: '', name: 'tomcat')
        booleanParam(defaultValue: false, description: '', name: 'mysql')
        booleanParam(defaultValue: false, description: '', name: 'postgres')
   }
    



    stages {
        stage('git'){
  steps {      
        git 'https://github.com/naniishan/ass.git'
}}
        stage("foo") {
            steps {
                echo "flag: ${params.java}"
                echo "flag: ${params.tomcat}"
                echo "flag: ${params.nginx}"
          
            }
        }
        
          stage('Speak'){
            when {
                // Only say hello if a "greeting" is requested
                expression { params.java == true }
            }
            steps {
                sh 'ansible-playbook java.yml'}
 }
        
        stage('Spedhdhak'){
            when {
                // Only say hello if a "greeting" is requested
                expression { params.nginx == true }
            }
            steps {
                sh 'ansible-playbook nginx.yml'

            }
        }
        stage('Spedhdhakvxcvxcvxvc'){
            when {
                // Only say hello if a "greeting" is requested
                expression { params.tomcat == true }
            }
            steps {
                sh 'ansible-playbook tomcat.yml'

            }

        }

 stage('Spedhdhakvxcvxcsdfdsfvxvc'){
            when {
                // Only say hello if a "greeting" is requested
                expression { params.mysql == true }
            }
            steps {
                sh 'ansible-playbook mysql.yml'

            }
        }














    }

    }
