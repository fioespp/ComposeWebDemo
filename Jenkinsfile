
pipeline {
    agent any

    stages {
        stage('1 - Tests') {
            steps {
                bat './gradlew.bat :shared:wasmJsTest'
            }
        }

        stage('2 - Build WebAssembly') {
            steps {
                bat './gradlew.bat :webApp:wasmJsBrowserDistribution'
            }
        }
    }
}
