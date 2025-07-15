pipeline {
  agent any

  stages {
    stage('Build qwer') {
      when {
        changeset "**/qwer/**"
      }
      steps {
        echo "qwer 디렉토리에 변경사항이 있을때만 빌드 실행"
        // 예: 빌드 스크립트 실행
        //sh './your-directory/build.sh'
      }
    }
    stage('Build asdf') {
      when {
        changeset "**/asdf/**"
      }
      steps {
        echo "qwer 디렉토리에 변경사항이 있을때만 빌드 실행"
      }
    }
  }
}
