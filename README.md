# StopEC2InstanceByTag
For your test/dev AWS account, you can use this CloudFormation template to create a scheduled CloudWatch task to stop running EC2 instances after work to save money, as long as those EC2 instances have a tag "AutoOff" with value "True". I create short-lived AWS dev/test accounts and their lifespan is only one week. This CloudFormation template is pretty useful for that purpose.

By default, the EC2 instances will be stopped at 11:00PM GMT. You can modify the associated CloudWatch rule to have it running at a different time.

Lambda source code embedded in this CloudFormation template was copied from https://gist.github.com/mlapida/1917b5db84b76b1d1d55, on Aug 7, 2018
