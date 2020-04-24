pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        sh '''pipeline {
  agent any
  stages {
    stage(\'Upload to AWS\') {
      steps {
        sh \'echo "Hello World"\'
        sh \'\'\'
					 echo "Multilines shell steps works too"
					 ls -lah
					 \'\'\'
				}
			}
		}
    }'''
        }
      }

      stage('Lint HTML') {
        steps {
          sh 'tidy -q -e *.html'
        }
      }

    }
  }