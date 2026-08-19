pipeline {
    agent {
label{
  label 'slave-1' 
}
}
stages {
  stage('Deploy on slave-1'){         
    steps {
                
                   sh 'rm -rf *'
                   sh 'git clone https://github.com/divyakgit/R3.git'
                    sh 'sudo yum install -y httpd'
                    sh 'sudo systemctl start httpd'
                    sh 'sudo cp index.html /var/www/html/index.html'
                
            }
        }
}
}


