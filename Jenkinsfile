 def workspace;
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '91cd487b-19fe-4b36-94ee-5064334e9fe3', url: 'https://github.com/tarugusatish1/maven.git']]])  
        workspace =pwd()
        
    }
    stage('static code analysis')
    {
        echo "static code analysis"
        
    }
    stage('Build')
    {
        echo "build the code"
    }
    stage('Unit Testing')
    {
        echo "Unit testing"
    }
    stage('Delivery')
    {
        echo "Deliver the code"
    }
        
}
    
