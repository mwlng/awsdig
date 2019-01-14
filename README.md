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
   > $ chown +x awsdig

3. Run "./awsdig help" to print usage and help messages

## Plugins

Download links
* macOS \
  [ami](https://drive.google.com/uc?export=download&id=17Jp9vlhhDki6_yNgXKMBHvMVeEcWeJ7Q)
  [cloudformation](https://drive.google.com/uc?export=download&id=1jElLafFCoLvjKL1WI7lHkyfXQGR6B4y8)
  [emr](https://drive.google.com/uc?export=download&id=15foHYERbIGbU9s-vEm1DBjJxwSP0dpDz)
  [iam](https://drive.google.com/uc?export=download&id=1Dm1b3SOfRJsUZJYL1CyPVm8kuTaYEe98)
  [route53](https://drive.google.com/uc?export=download&id=11XKVIcfq09oELh6WVP_fZaXz-V1QhC4I)

* Linux \
  [ami](https://drive.google.com/uc?export=download&id=1xwPu9ATGvwzSxu_nPVc-MOMV3XanPiDw)
  [cloudformation](https://drive.google.com/uc?export=download&id=1jUdv_WrmCFniwU9h-m_TvAB0W2WUTLWC)
  [emr](https://drive.google.com/uc?export=download&id=1ltZxRLPtZOS_ra_W2RWuBNvTH0mtUZiF)
  [iam](https://drive.google.com/uc?export=download&id=1CnA93jvkiHcHJdKw5f1Ik_uqYW9wmak6)
  [route53](https://drive.google.com/uc?export=download&id=1CnA93jvkiHcHJdKw5f1Ik_uqYW9wmak6)

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
