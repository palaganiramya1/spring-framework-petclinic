node("GOL1") {
        stage("git") {
            git url: 'https://github.com/palaganiramya1/spring-framework-petclinic.git',
                branch: 'REL_INT_1.0'
        }
       stage("build") {
        sh '/usr/share/maven/bin/mvn package'
        } 
       stage('results') {
        junit '**/surefire-reports/*.xml'
       } 
    }
