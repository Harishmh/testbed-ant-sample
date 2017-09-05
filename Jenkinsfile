pipeline {
    agent any
	stages {
	    stage ('Prepare environment') {
        			steps {
        				withMaven(maven : 'apache-maven') {
                             bat 'mvn clean compile'
        					 }
        					}
        				}
        stage ('Compile Stage') {
			steps {
				withMaven(maven : 'apache-maven') {
                     bat 'mvn clean compile'
					 }
					}
				}
				stage ('Testing Stage') {


                                steps {
                                        withMaven(maven : 'apache-maven') {
                                                                    bat 'mvn test'
                                                                }

                        }
                 stage ('Deployment2 Stage') {
                                             steps {
                                                 withMaven(maven : 'apache-maven ') {
                                                     bat 'mvn deploy'
                                                 }
                                             }
                                         }
			}
		}