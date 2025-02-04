pipeline
{
  agent any

  stages
  {
    stage('Build')
{
  steps
  {
    echo 'Build App'
  }
}

stage('Test')
{
  steps
  {
    echo 'Test App'
  }
}
stage('Deploy')
{
  steps
  {
    echo 'Deploy APP'
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
