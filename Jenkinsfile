pipeline {
  agent any

  stages {
    stage('Build qwer') {
      when {
        anyOf {
          changeset "**/qwer/**"
          expression { return env.BUILD_NUMBER == '1' }
        }
      }
      steps {
        echo "qwer 디렉토리에 변경사항이 있을때만 빌드 실행"
        // 예: 빌드 스크립트 실행
        //sh './your-directory/build.sh'
      }
    }
    stage('Build asdf') {
      when {
        anyOf {
          changeset "**/asdf/**"
          expression { return env.BUILD_NUMBER == '1' }
        }
      }
      steps {
        echo "asdf 디렉토리에 변경사항이 있을때만 빌드 실행"
      }
    }
  }
}
