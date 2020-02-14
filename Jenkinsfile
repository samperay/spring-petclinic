pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                sh 'cd spring-petclinic; ./mvnw package' 
            }
        }
        stage('Copy Artefact'){
            steps {
                sh 'sudo cp target/spring-petclinic-*.jar /mnt/artefact'
            }
        }
    }
}
