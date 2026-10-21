pipeline { 
      agent any
      stages {
          stage('Checkout'){
            steps {
                checkout scm
            }
          }
      stage('Install Dependencies'){
          steps {
             sh '''
                  python3 -m venv venv 
                  venv/bin/pip install -r requirements.txt
             '''
          }
      }
      stage('Run Test')
cat > Jenkinsfile <<'EOF'
pipeline { 
      agent any
      stages {
          stage('Checkout'){
            steps {
                checkout scm
            }
          }
      stage('Install Dependencies'){
          steps {
             sh '''
                  python3 -m venv venv 
                  venv/bin/pip install -r requirements.txt
             '''
          }
      }
      stage('Run Test'){

       steps {
             sh 'docker build -t python-cicd:v1 .'
       }
    }
  }
}
'EOF'

cat > Jenkinsfile <<'EOF'
pipeline { 
      agent any
      stages {
          stage('Checkout'){
            steps {
                checkout scm
            }
          }
      stage('Install Dependencies'){
          steps {
             sh '''
                  python3 -m venv venv 
                  venv/bin/pip install -r requirements.txt
             '''
          }
      }
      stage('Run Test')
cat > Jenkinsfile <<'EOF'
pipeline { 
      agent any
      stages {
          stage('Checkout'){
            steps {
                checkout scm
            }
          }
      stage('Install Dependencies'){
          steps {
             sh '''
                  python3 -m venv venv 
                  venv/bin/pip install -r requirements.txt
             '''
          }
      }
      stage('Run Test'){

       steps {
             sh 'docker build -t python-cicd:v1 .'
       }
    }
  }
}
