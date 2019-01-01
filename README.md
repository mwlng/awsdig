# awsdig

## Overview

awsdig is an interactive command line tool for people to dig into AWS resources more easily than using AWS web console. 

## Prerequisite
It requires AWS account and AWS CLI credentials to be setup on your computer.

https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html

## Binary downloads

* macOS \
  [64-bit](https://drive.google.com/open?id=1oQfcN93aBFuAd86SovgtvgUHtm6Drs_X)
* Linux \
  [64-bit](downloads/linux/64/awsdig.tgz)
* Windows \
  [64-bit](donwloads/win/65/awsdig.zip)

## Installation
1. Use the above links to download correct version of awsdig binary for your OS.
2. Uppack downloaded arhcive

   For macOS|Linux
   > $ tar -xvf awsdig.tgz \
   > $ cd awsdig \
   > $ chown +x awsdig

   For Windows, reference to Winodws manual. 
3. Directory layout
    
       awsdig/
        ├── awsdig
        └── plugins
            └── aws
                ├── ami.plugin
                ├── emr.plugin
                └── iam.plugin
    All plugins should have 'plugin' file extension, and should be put inside cloud provider folder(ie: aws) which is under plugings directory.
4. Run "./awsdig help" to print usage and help messages

Have fun and enjoy!!!

-----
Note: This project is heavily developing, No PRs will be accepted at this moment.
