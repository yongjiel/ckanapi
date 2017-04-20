=============
Changes from ckanapi version 3.6
=============

1. change _upload_resources function of cli/load.py:

    Add resource id from package dataset when upload resources

2. Change extract_ids_or_names funtion of cli/delete/py:

    Return name first instead of ID. For the remote system, the 
    ID should be different with the current system. But the name
    should be the same.

3. Change _request_fn and _request_fn_get functions of remoteckan.py;
    
    Add verify=False when call requests. Our UAT server side with SSL 
    self-signed centifcate. Should turn off the verification when call
    outside of server.



