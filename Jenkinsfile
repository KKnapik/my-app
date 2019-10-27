
node {
   stage('SCM checkout'){
      git 'https://github.com/KKnapik/my-app.git'
   }
   stage('Compaile package'){
      sh 'mvn package'
   }
}