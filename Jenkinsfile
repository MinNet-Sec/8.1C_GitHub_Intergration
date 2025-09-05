pipeline {
  agent any
  options {
    timestamps()
  }

  stages {
    stage('Build') {
      steps {
        echo 'Build: compile or package the source code (e.g., Maven/Gradle).'
      }
    }

    stage('Unit & Integration Tests') {
      steps {
        echo 'Tests: run unit and integration tests.'
      }
    }

    stage('Code Analysis') {
      steps {
        echo 'Code Analysis: run static code quality tools (e.g., SonarQube).'
      }
    }

    stage('Security Scan') {
      steps {
        echo 'Security Scan: run SAST/SCA tools to detect vulnerabilities.'
      }
    }

    stage('Deploy to Staging') {
      steps {
        echo 'Deploy to Staging: deliver artifacts to the staging environment.'
      }
    }

    stage('Integration Tests on Staging') {
      steps {
        echo 'Staging Tests: execute end-to-end/integration tests against staging.'
      }
    }

    stage('Deploy to Production') {
      steps {
        echo 'Deploy to Production: release the approved build to production.'
      }
    }
  }

  post {
    always {
      echo 'Pipeline completed.!!! check Change and auto-build'
    }
  }
}

