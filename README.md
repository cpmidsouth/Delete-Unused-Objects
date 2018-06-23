This script will search your object database for unused objects. It will output a deletion commands file to clean those up. Both SMS and MDS are supported in the same script.

You have two options of use; NAME or UID.

## Please be careful when using any API tool to modify your database. Be sure to verify all data ##


## How to use ##
 - cp script over to mgmt station (this script is intended to run directly on the mgmt station)
 - execute ./script-name.sh
    - script will ask for IP of SMS or Domain of MDS you wish to search
 - Output will be in delete-unused-objects.txt
    - delete-unused-objects.txt will have the mgmt_cli commands for deletion. If you want to execute it do the following;
      - chmod 755 delete-unused-objects.txt
      - ./delete-unused-objects.txt
