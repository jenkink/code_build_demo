pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          awsCodeBuild projectName: 'code-build-demo-kj',
                       credentialsId: 'code-build-demo',
                       credentialsType: 'jenkins',
                       region: 'us-east-1',
                       sourceControlType: 'project'

        }
      }
    }
}
