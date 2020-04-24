pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        sh 'echo "Hello World"'
        sh '''
					 echo "Multilines shell steps works too"
					 ls -lah
					 '''
      }	    withAWS(credentials: 'aws-credentials', region: 'us-west-2') {
    sh 'aws iam get-user'
}
}
    }

  }
}
