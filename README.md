# codespaces-test
Testing out codespaces and deploying Azure resource using bicep

Prequisites
1. az cli installed (Below command is for Linux machines)
    ```
    curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
    ```
2. login to azure

Steps
1. Create the .bicep file and specify the resources we want to create
2. Compile the .bicep file into an ARM template of extension .json
    ```
    az bicep build --file <filename>.bicep
    ```
3. Deploy the ARM template
    ```
    az deployment group create --resource-group <resource group name> --template-file <filename>.json
    ```
4. Tadaaa