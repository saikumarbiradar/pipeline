pipeline {
	agent any  
	stages {
		stage('BUILD') {
			parallel {
				stage('build1') {
					steps {
						sh 'ls'
					}
				}
				stage ('build2') {
					steps {
						sh 'pwd'
					}
				}
			}
		}
		
		stage('TEST') { 
			parallel {
				stage('TEST1') {
					steps {
						sh 'sleep 5'
					}
				}
				stage('TEST2') {
					steps {
						sh 'sleep 5'
					}
				}
				stage('TEST3') {
					steps {
						sh 'sleep 5'
					}
				}
				stage('TEST4') {
					steps {
						sh 'sleep 5'
					}
				}
			}
		}
				

		
		stage('DEPLOY') {
		       parallel {
			       stage ('DEPLOY1') {
				       steps {
					       sh 'ls'
				       }
			       }
			       stage ('DEPLOY2') {
				       steps {
					       sh 'sleep 5'
				       }
			       }
			       stage ('DEPLOY3') {
				       steps {
					       sh '''
					       pwd
					       ls -lrt
					       echo this is third deploy stage
					       '''
				       }
			       }
		       }
		}
	}
}
		
         

