pipeline { 
    agent any 
        stage('Build') { 
            steps { 
                sh './mvwn clean package'
            }
        }

        stage('Copy Artifact'){
            steps {
                sh 'sudo cp -rvf target/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar /mnt/artefact/'
            }
        }
}
