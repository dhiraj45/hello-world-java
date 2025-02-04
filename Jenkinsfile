pipeline {
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}

post
{
  always
  {
    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
      echo 'Post build actions will run if configured'
      echo "Build result: ${buildResult}"
      echo "Stage result: ${stageResult}"
    }
  }
}
}
