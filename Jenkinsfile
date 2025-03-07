pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "Building the Application..."
            }
        }
 
    }
    post {
        // Only run when the current pipeline or specific stage has success 
        success {
            echo "# POST  ===> SUCCESFULLY Triggered"
        }
        // this will run only when the current pipeline or stage has failed
        failure {
            echo "# POST  ===> FAILURE Triggered"
        }
        // this will run regardless of the pipeline status
        always {
            echo "# POST  ===> ALWAYS Triggered"
        }
    }
}
