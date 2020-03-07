pipeline {
  agent any
  stages {
    stage('Start') {
      steps {
        writeFile(file: 'tmp.txt', text: 'Abc')
      }
    }

    stage('Git') {
      steps {
        sleep 10
        retry(count: 5) {
          echo '"Hehehe"'
        }

      }
    }

  }
}