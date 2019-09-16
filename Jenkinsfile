
#!/usr/bin/env groovy

import hudson.model.*
import hudson.EnvVars
import java.net.URL

node{
stage('git checkout') {

git 'https://github.com/shubham5105/DevOpsClassCodes.git'
}

stage('compile'){
    withMaven(maven:'mymaven'){
        sh 'mvn compile'

}}

stage('package') {
    withMaven(maven:'mymaven'){
         sh 'mvn package'
}}}
