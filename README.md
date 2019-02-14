# awsdig

## Overview

awsdig is an interactive command line tool for people to dig into AWS resources more easily than using AWS web console. 

## Prerequisite
It requires AWS account, and AWS CLI credentials to be setup on your computer.

Use below link for first time setup or details

https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html

## Binary downloads

* macOS \
  [64-bit](https://drive.google.com/uc?export=download&id=1NXPTuuTF2u72fehHL0SCB4B9PmQd_NwB)
* Linux \
  [64-bit](https://drive.google.com/uc?export=download&id=1h1QfVWkgJry7lJO_QnaTTxh2oAgsl7Ne)
* Windows \
  [Under implementation]

## Installation
1. Use the above links to download correct version of awsdig binary for your OS.
2. Uppack downloaded arhcive

   For macOS|Linux
   > $ tar -xvf awsdig.tgz \
   > $ cd awsdig \
   > $ chmod +x awsdig


    Directory layout

       awsdig/
        ├── awsdig
        └── plugins
            └── aws
                ├── ami.plugin
                ├── cloudformation.plugin
                ├── emr.plugin
                ├── iam.plugin
                └── ...


3. Run "./awsdig help" to print usage and help messages

## Plugins

Currently, awsdig has impelemented plugins for below AWS resources.

* ami
* autoscaling
* cloudformation
* ec2-instances
* ecs
* emr
* glue
* iam
* route53

You can download the source code from https://github.com/mwlng/awsdig-plugins 

All plugins should have 'plugin' file extension, and should be put inside cloud provider folder(ie: aws) which is under plugings directory.

## Usage

Command List:

    ls      List available services or resources under current context/path
    cd      Change service's context or resource's path
    cat     Print resource's attributes/content
    clear   Clear screen
    help    Print usage and help messages
    exit    Exit this program

Others:

    tab     For command auto-completion
     |      Pipe command's output to external programs or shell commands


Have fun and enjoy !!!


-----
Note: This project is heavily developing, No PRs will be accepted at this moment.
