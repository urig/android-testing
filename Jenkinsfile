pipeline {
  agent {
    // Run on a build agent where we have the Android SDK installed
    label 'android'
  }
  buildScan { licenseAgreementUrl = 'https://gradle.com/terms-of-service'; licenseAgree = 'yes' }
  stages {
    stage('Compile') {
      steps {
        // Compile the app and its dependencies
        sh './gradlew compileProdDebugSources --scan'
      }
    }
  }
}
