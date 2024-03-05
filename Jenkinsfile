node{
    stage('Git Chechout'){
      git url: 'https://github.com/bharathj0/star-agile-banking-finance/'
    }
    stage('Code Compile'){
      sh 'mvn compile'
    }
    stage('Code Test'){
      sh 'mvn test'
    }
    stage('Code Package'){
      sh 'mvn clean package'
    }
    stage('Run Docker File'){
            sh 'docker build -t bharathj0/Banking:1.0 .'
        }
  }

    
