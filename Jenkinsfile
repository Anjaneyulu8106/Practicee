pipeline {
    agent any

    parameters {
        choice(
            name: 'ENV',
            choices: ['DEV', 'QA', 'PROD'],
            description: 'Select deployment environment'
        )
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checkout completed'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application'
            }
        }

        stage('Test') {
    steps {
        echo "Running tests..."
        echo "All tests passed"
    }
}



        stage('Deploy') {
            steps {
                echo "Deploying application to ${params.ENV}"
            }
        }
    }
}
