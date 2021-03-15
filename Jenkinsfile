 pipeline {
     agent any
     stages {
        stage("Begin") {
            steps {
                echo 'Hello World'
                //git 'https://github.com/handuy/nodejs-todolist'
                
            }
        }
        stage("Send Result to email") {
            steps {
                emailext body: '''${DEFAULT_CONTENT}
${BUILD_LOG}
''', recipientProviders: [developers()], subject: '${DEFAULT_SUBJECT}', to: 'stevenguyenaz@gmail.com'
                
            }
        }
    }
}
