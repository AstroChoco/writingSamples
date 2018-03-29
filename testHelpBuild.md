# Test Help Build
1. Make a working branch of the downloaded project.
    ```
    cd test-frontend
    git branch <working_branch_name>
    ```
2. Switch to the working branch.
    ```
    git checkout <working_branch_name>
    ```
3. Copy the help file ```test.xml``` to the help folder and rename it to ```overview.xml```.

    ```
    cp test.xml systemSettings/help/en-us/systemsettings/overview.xml
    ```
4. Commit the help file ```overview.xml```.

    ```
    git add systemSettings/help/en-us/systemsettings/overview.xml
    git commit -m "system settings"    
    ```
