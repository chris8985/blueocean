pipeline {
  agent any
  stages {
    stage('build job') {
      steps {
        sh '''#!/bin/bash -x

#Get commit information 

COMPONENT_NAME="devops-test"
#export GIT_COMMIT=`git rev-parse HEAD`
#export GIT_SHORT_ID=${GIT_COMMIT:offset:5}
export TIME_STAMP=`date "+%Y%m%d%H%M"`
#export TARGET_NAME_TAG=${COMPONENT_NAME}-${TIME_STAMP}-${GIT_SHORT_ID}

echo `pwd`
echo `ls`
echo `which java`
echo `java -version`

echo `${COMPONENT_NAME}`
echo `${TIME_STAMP}`
echo "Job is done"
#git log --pretty=tformat: --numstat | gawk \'{ add += $1 ; subs += $2 ; loc += $1 + $2 } END { printf "added lines: %s removed lines : %s total lines: %s\\n",add,subs,loc }\''''
      }
    }
  }
}