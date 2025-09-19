stage('Clone GitHub Repo') {
    steps {
        script {
            echo 'Cloning GitHub repo to Jenkins...'
            checkout([
                $class: 'GitSCM',
                branches: [[name: '*/main']],
                userRemoteConfigs: [[
                    credentialsId: 'github-token',
                    url: 'https://github.com/Keshav-chand/Medical-RAG-Chatbot.git'
                ]]
            ])
        }
    }
}
