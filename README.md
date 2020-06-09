# AWS_Windows_VM
This is when a MacBook User need a Windows VM on AWS.

In your AWS CLI, type:
```
aws cloudformation create-stack \
--stack-name windowsbox \
--template-body file://windows_CF.yml \
--parameters ParameterKey=KeyName,ParameterValue=your_keyname \
             ParameterKey=VolumeSize,ParameterValue=30 \
```