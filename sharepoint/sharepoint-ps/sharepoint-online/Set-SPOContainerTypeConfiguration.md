---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: https://learn.microsoft.com/powershell/module/sharepoint-online/Set-SPOContainerTypeConfiguration
applicable: SharePoint Online
title: Set-SPOContainerTypeConfiguration
schema: 2.0.0
author: FarreltinF
ms.author: fanyi
ms.reviewer:
---

# Set-SPOContainerTypeConfiguration

## SYNOPSIS

Sets or updates the configuration settings of a container type in SharePoint Embedded.

## SYNTAX
```powershell
Set-SPOContainerTypeConfiguration [-ContainerTypeId <ContainerTypeId>] [-DiscoverabilityDisabled <Boolean>] [-SharingRestricted <Boolean>]
```

## DESCRIPTION

For any parameters passed in, the `Set-SPOContainerTypeConfiguration` cmdlet sets or updates the settings for a container type created under a SharePoint Embedded application.

You must be a SharePoint Administrator or Global Administrator to run this cmdlet.

## EXAMPLES

### Example 1

```powershell
Set-SPOContainerTypeConfiguration -ContainerTypeId 4f0af585-8dcc-0000-223d-661eb2c604e4 -DiscoverabilityDisabled $false
```

Example 1 turns on discoverability for this container type. All content created within this container type will be discoverable in the Microsoft 365 experience, including on office.com, onedrive.com, recommended files, and other intelligent discovery experiences.

### Example 2

```powershell
Set-SPOContainerTypeConfiguration -ContainerTypeId 4f0af585-8dcc-0000-223d-661eb2c604e4 -SharingRestricted $false
```

Example 2 turns on an open sharing model for this container type. Any container members and guest users with edit permissions can share files created within the container type.

## PARAMETERS

### -DiscoverabilityDisabled

As a SharePoint Administrator or Global Administrator in Microsoft 365, you can control how your content appears in the Microsoft 365 experience. The default value for this parameter is True, which hides the SharePoint Embedded application content throughout the Microsoft 365 environment, including on office.com, onedrive.com, in recommended sections, or through other Microsoft intelligent file discovery features.
If you opt into the Microsoft 365 experience, your files will be integrated into Microsoft 365 environment, participating in intelligent file discovery.

PARAMVALUE: $true | $false

```yaml
Type: Boolean
Position: Named
Required: False
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
Applies to: SharePoint Embedded
```

### -SharingRestricted

SharePoint Embedded offers a role-based sharing model that allows developers to configure file-sharing permissions based on container permission roles, offering a choice between a restrictive and an open sharing model. The open sharing model allows any container members and guest users with edit permissions to share files. The restrictive sharing model allows only container members who are either Owners or Managers to share files.
 
PARAMVALUE: $true | $false

```yaml
Type: Boolean
Position: Named
Required: False
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
Applies to: SharePoint Embedded
```

## RELATED LINKS

[Get-SPOContainerTypeConfiguration](Get-SPOContainerTypeConfiguration.md)
