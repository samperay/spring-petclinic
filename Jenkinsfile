pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                sh './mvnw package' 
            }
        }
        stage('Copy Artefact'){
            steps {
                sh 'sudo cp target/spring-petclinic-*.jar /mnt/artefact'
            }
        }
    }
}
