node{
   stage('SCM checkout'){
     git 'https://github.com/tarugusatish1/maven/new/master'
     }
   stage('compile-package') {
    def mvnHOME =     tool name: 'maven', type: 'maven'
      sh "${mvnHOME}/bin/mvn package"
     }
     
}   
