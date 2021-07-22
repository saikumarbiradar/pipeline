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
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: DEPLOY
				'''
			}	
		}
	}
}
