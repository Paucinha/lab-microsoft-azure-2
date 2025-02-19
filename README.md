# Criando máquinas Virtuais na Azure

![GitHub](https://img.shields.io/github/license/Paucinha/api-ecommerce-dio?style=flat-square)

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO, como a nuvem pode melhorar a eficiência e escalabilidade:

- Benefícios da alta disponibilidade e da escalabilidade na nuvem.
  
- Benefícios da confiabilidade e da previsibilidade na nuvem.
  
- Benefícios da segurança e da governança na nuvem.
 
- Benefícios da capacidade de gerenciamento na nuvem.

**Azure | Full-Stack | Básico**

- [Criação da Máquina Virtual na Azure no Portal Microsoft Azure](https://portal.azure.com/#create/Microsoft.VirtualMachine)

```json  
{
    "name": "my-Vm-1",
    "id": "/subscriptions/f5f6088e-679a-4fc3-9a5d-600dcca616e6/resourceGroups/my-Vm-1_group/providers/Microsoft.Compute/virtualMachines/my-Vm-1",
    "type": "Microsoft.Compute/virtualMachines",
    "location": "eastus",
    "properties": {
        "hardwareProfile": {
            "vmSize": "Standard_D2s_v3"
        },
        "provisioningState": "Updating",
        "vmId": "1c25eb45-158d-4157-b561-e9ee2a905dea",
        "additionalCapabilities": {
            "hibernationEnabled": false
        },
        "storageProfile": {
            "imageReference": {
                "publisher": "canonical",
                "offer": "ubuntu-24_04-lts",
                "sku": "server",
                "version": "latest",
                "exactVersion": "24.04.202502040"
            },
            "osDisk": {
                "osType": "Linux",
                "name": "my-Vm-1_disk1_4196511456b741f9892a69e8e876ed1d",
                "createOption": "FromImage",
                "caching": "ReadWrite",
                "managedDisk": {
                    "id": "/subscriptions/f5f6088e-679a-4fc3-9a5d-600dcca616e6/resourceGroups/my-Vm-1_group/providers/Microsoft.Compute/disks/my-Vm-1_disk1_4196511456b741f9892a69e8e876ed1d"
                },
                "deleteOption": "Delete"
            },
            "dataDisks": []
        },
        "osProfile": {
            "computerName": "my-Vm-1",
            "adminUsername": "azureuser",
            "linuxConfiguration": {
                "disablePasswordAuthentication": true,
                "ssh": {
                    "publicKeys": [
                        {
                            "path": "/home/azureuser/.ssh/authorized_keys",
                            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCnqz06ecLC9/eK/FGuuhqw6prnRndyaZS1T3mld25TXr0iQX60JIoO53EqydxeGPV9yx+ryF5ghQJPlR9nZyY9q6+8k+YozopBoGN5IJymhGwngo/HnT5meKpw9Jp9fyEBUUj1ASRU4GhX6Mx4tobtyMVMlEDB+LRuJQbVX3vKbJ/1IgjBXdbDQ0HsJgBYqZrxLLkFwuzXJOsYsqqEMOscKpE6SAvnrj0RRaD7XAKmF/HpHO81Nm7oi/goUzLsAOCM/SFIgB/ORqMqbBB4edwMb6UY1heonwhTBrVI4a9chQWN6sxyHf2Vve0YwgqRR4/9F8br6+zORGhKtZXlXiC1JPar7yBVzBovUg+MhNiee1Bf+m6YxlgE1HnEQM3HX0gxiOG903yWPhb637loLHN0vVpZFnPkFlEE/NgZoYcvBanGdVmV0KEPAJFQZAcUO+QYYmKgPs5KULRKz/7VJdgRxGgqJwbB4Cz9p+EXWDL6JBIze7ZnGHl23qupdOHlRf0= generated-by-azure"
                        }
                    ]
                },
                "provisionVMAgent": true,
                "patchSettings": {
                    "patchMode": "ImageDefault",
                    "assessmentMode": "ImageDefault"
                }
            },
            "secrets": [],
            "allowExtensionOperations": true,
            "requireGuestProvisionSignal": true
        },
        "securityProfile": {
            "uefiSettings": {
                "secureBootEnabled": true,
                "vTpmEnabled": true
            },
            "securityType": "TrustedLaunch"
        },
        "networkProfile": {
            "networkInterfaces": [
                {
                    "id": "/subscriptions/f5f6088e-679a-4fc3-9a5d-600dcca616e6/resourceGroups/my-Vm-1_group/providers/Microsoft.Network/networkInterfaces/my-vm-12_z3",
                    "properties": {
                        "deleteOption": "Detach"
                    }
                }
            ]
        },
        "diagnosticsProfile": {
            "bootDiagnostics": {
                "enabled": true
            }
        }
    },
    "zones": [
        "3"
    ],
    "apiVersion": "2021-03-01"
}
```

##

Projeto desenvolvido durante o [**Bootcamp Bradesco - Java Cloud Native**](https://www.dio.me/bootcamp/bradesco-java-cloud-native), fornecido pela [**DIO**](https://www.dio.me/)

##

- [By Páucinha](https://github.com/Paucinha)
