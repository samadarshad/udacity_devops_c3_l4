udacity_devops_c3_l4

https://github.com/jrrobles979/cdond-c3-projectstarter/blob/master/.circleci/config.yml


source env/bin/activate    
export AWS_DEFAULT_PROFILE=udacity


aws cloudformation deploy --template-file cloudfront.yml --stack-name production-distro --parameter-overrides PipelineID="568947551106-c3-l4" --tags project=udapeople &