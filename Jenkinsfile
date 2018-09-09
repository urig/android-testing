pipeline {
  agent {
    // Run on a build agent where we have the Android SDK installed
    label 'android'
  }
  stages {
    stage('Compile') {
      steps {
        // Compile the app and its dependencies
        sh './gradlew compileDebugSources'
      }
    }
  }
}
