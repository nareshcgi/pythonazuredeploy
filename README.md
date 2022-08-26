# pythonazuredeploy
Testing Python Django deploy in Azure Web App service.

# Upload files to Gitlab registry
curl --header "PRIVATE-TOKEN: glpat-84rso_RzrikD5Tss" --upload-file samplepythonapp-0.1.zip  "https://gitlab.com/api/v4/projects/29861801/packages/generic/testpackage/1.0.0/samplepythonapp.zip?status=default&select=package_file"

where 
    glpat-84rso_RzrikD5Tss is the gitlab access token 
    testpackage is the package name (use this to upload multiple files related to the same app)
    29861801 is the project id
    1.0.0 version
    status use default so that it shows up in UI, you can also specify hidden
    select=package_file gives metadata about the uploaded file

