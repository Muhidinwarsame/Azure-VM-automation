# how to Azure automate VM using Powershell, please use commands  from step 2-10 to create virtual machines.
New-AzVm `
    -ResourceGroupName "MYDEMO01" `
    -Name "MYVM01" `
    -Location "East US" `
    -VirtualNetworkName "MYVNET" `
    -SubnetName "MYSubnet" `
    -SecurityGroupName "MYNSG" `
    -PublicIpAddressName "myPublicIpAddress" `
    -OpenPorts 80,3389
