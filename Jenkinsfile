pipeline {
	agent {
		label 'ubuntu'
		}
	stages {
		stage ("pull scm python") {
			steps {
				git branch: 'python', url: 'https://github.com/duveykrishna/Python-pipeline.git'
				}
			}
		stage ("Build") {
			steps {
				sh 'python3 -V'
				sh 'python3 cp.py'
				}
			}
		stage ("Test") {
			steps {
				sh 'python3 test.py'
				}
			}
		}
	}
