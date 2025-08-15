
stage('Build') {
  parallel {
    stage('Build Frontend') {
      steps {
        sh 'cd frontend && npm install && npm run build'
      }
    }
    stage('Build Backend') {
      steps {
        sh 'cd backend && ./gradlew build'
      }
    }
  }
}
