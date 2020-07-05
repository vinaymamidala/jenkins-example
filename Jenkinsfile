pipeline {
    agent any
    
    def mavenHome = tool name: "maven3.6.3"

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven3.6.3') {
                    sh '${mavenHome}/bin/mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven3.6.3') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'maven3.6.3') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
