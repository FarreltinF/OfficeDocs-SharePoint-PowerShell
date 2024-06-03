---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: https://learn.microsoft.com/powershell/module/sharepoint-online/Get-SPOContainertypeConfiguration
applicable: SharePoint Online
title: Get-SPOContainerTypeConfiguration
schema: 2.0.0
author: FarreltinF
ms.author: fanyi
ms.reviewer:
---

# Get-SPOContainertypeConfiguration

## SYNOPSIS

Returns container type configurations in a SharePoint Embedded application. 

## SYNTAX

### ParamSet1

```powershell
Get-SPOContainerTypeConfiguration [-ContainerTypeId <ContainerTypeId>]
```

## DESCRIPTION

The `Get-SPOContainerTypeConfiguration` cmdlet retrieves and returns configuration settings set on a container type created under a SharePoint Embedded application. 

You must be a SharePoint Administrator or Global Administrator to run this cmdlet.

## EXAMPLES

### Example 1

```powershell
Get-SPOContainerTypeConfiguration -ContainerTypeId 4f0af585-8dcc-0000-223d-661eb2c604e4  
```

This example returns a list of configurations set on a container type '4f0af585-8dcc-0000-223d-661eb2c604e4'.

## PARAMETERS

### -ContainerTypeId

This parameter specifies the ID of the SharePoint Embedded container type. Use the `Get-SPOContainerType` command to retrieve the ContainerTypeId.
 
```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[Set-SPOContainerTypeConfiguration](Set-SPOContainerTypeConfiguration.md)

