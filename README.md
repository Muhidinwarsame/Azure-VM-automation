# How to automate azure VM using Powershell.
New-AzVm `
    -ResourceGroupName "MYDEMO01" `
    -Name "MYVM01" `
    -Location "East US" `
    -VirtualNetworkName "MYVNET" `
    -SubnetName "MYSubnet" `
    -SecurityGroupName "MYNSG" `
    -PublicIpAddressName "myPublicIpAddress" `
    -OpenPorts 80,3389
