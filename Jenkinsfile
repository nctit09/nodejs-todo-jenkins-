 pipeline {
     agent any
     stages {
          stage("Hello") {
               steps {
                    echo 'Hello World'
                    //git 'https://github.com/handuy/nodejs-todolist'
                    
            }
        stage("Send Result to email") {
            steps {
                emailext body: 'alo alo', recipientProviders: [developers()], subject: 'Test ABC', to: 'stevenguyenaz@gmail.com'
                
            }
        }
}
}
}