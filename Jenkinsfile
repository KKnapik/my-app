
node {
   stage('SCM checkout'){
      git 'https://github.com/KKnapik/my-app.git'
   }
   stage('Compaile package'){
      def mvnHome = tool name: 'maven-3', type: 'maven'
      sh "${mvnHome}/bin/mvn package" 
   }
   stage{
     mail bcc: '', body: 'yo yo jenkins here ! ', cc: '', from: '', replyTo: '', subject: '', to: 'kr.knapik@gmail.com'
   }
}