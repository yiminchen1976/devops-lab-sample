node {
    stage('init'){
        checkout scm
    }
    stage('build'){
        sh 'cd sample/pipeline-as-code && mvn package'
    }
    stage('exec'){
        sh 'cd sample/pipeline-as-code && java -cp target/hello-1.0.jar com.systex.HelloWorld'
    }
}
