pipeline{
    agent {
        kubernetes{
            yaml '''
apiVersion: v1
kind: Pod
spec:
  containers:
  - name: shell
    image: maven
    command:
    - sleep
    args:
    - infinity
'''
            defaultContainer 'shell' 
        }
    }
        stages{
            stage("print changeset"){
                steps{
                    script{
                        println currentBuild.changeSets[0].getLogs()[0].getAuthor()
                    }
                }
            }
            stage("Run Mock Load")
            {
                parallel{
                    stage("Load 1"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 2"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 3"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 4"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 5"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 6"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 7"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 8"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 9"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 10"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 11"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 12"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 13"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                     stage("Load 14"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 15"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 16"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 17"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                    stage("Load 18"){
                        steps{
                        mockLoad 120
                        junit 'mock-junit.xml'
                        }
                    }
                }
            }
        }
}