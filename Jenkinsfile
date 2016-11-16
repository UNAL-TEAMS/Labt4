#!groovy

node {

    try {

       stage 'Checkout'
            // properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('H/15 * * * *')])])
            checkout scm

       stage 'Test'

            env.NODE_ENV = "test"

            print "Environment will be : ${env.NODE_ENV}"
       }


    catch (err) {

        throw err
    }

}
