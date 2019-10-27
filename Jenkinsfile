
node {
   stage('SCM checkout'){
      git 'https://github.com/KKnapik/my-app.git'
   }
   stage('Compaile package'){
      def mvnHome = tool name: 'maven-3', type: 'maven'
      sh "${mvnHome}/bin/mvn package" 
   }
   stage('Mail notification'){
     mail bcc: '', body: 'yo yo jenkins here ! ', cc: '', from: '', replyTo: '', subject: 'build', to: 'kr.knapik@gmail.com'
   }
}