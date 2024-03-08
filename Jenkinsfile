pipeline{
    agent{
        label "jenkins-agent"
    }
    tools {
        jdk 'Java21'
        maven 'Maven3'
    }
    stages{
        stage("Cleanup Workspace"){
            steps {
                echo "======executing A========="
                cleanWs()
            }
        }
    }

        stages{
        stage("Checkout from SCM"){
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/RazielSa/jenkins'
            }
        }
    }

}g