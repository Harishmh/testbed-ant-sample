pipeline {
    agent any

   stages {
        stage ('Prepare environment') {

            steps {
                env.PATH = "${tool 'Ant'}/bin:${env.PATH}"
                     bat 'ant -version'
					bat 'java -version'
                }
            }
        }
   }