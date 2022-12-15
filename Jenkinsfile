pipeline {
    ...output omitted...
    stages {
        stage('Run Tests') {
            ...output omitted...
        }
        stage('Deploy') {
            when {
                expression { env.GIT_BRANCH == 'origin/main' }
            }
            beforeInput true
        }
        input {
            message 'Deploy the application?'
        }
            steps {
                echo 'Deploying...'
            }
        }
    }
}
