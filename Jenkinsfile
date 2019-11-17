pipeline {
    agent any

    stages {
        stage("Checkout") {
            steps {
                checkout scm
            }
        }

        stage("Setup") {
            steps {
                sh "echo \"sdk.dir=${env.ANDROID_HOME}\" > local.properties"
            }
        }
    }
}
