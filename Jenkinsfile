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
    emailext body: 'summary', subject: 'Pipeline Status', to: 'c0930056@mylambton.ca'
  }
}
}
