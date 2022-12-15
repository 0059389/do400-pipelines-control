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
            steps {
                echo 'Step not executed...''
            }
        }
    }
}
