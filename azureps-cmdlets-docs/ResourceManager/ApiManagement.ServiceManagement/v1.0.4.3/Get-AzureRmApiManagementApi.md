---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version:
schema: 2.0.0
---

# Get-AzureRmApiManagementApi

## SYNOPSIS
Gets one or more APIs.

## SYNTAX

### All APIs (Default)
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> [<CommonParameters>]
```

### Find by ID
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> -ApiId <String> [<CommonParameters>]
```

### Find by Name
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> -Name <String> [<CommonParameters>]
```

### Find by product ID
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> -ProductId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApiManagementApi** cmdlet gets one or more APIs.

## EXAMPLES

### Example 1: Get all APIs
```
PS C:\> Get-AzureRmApiManagementApi -Context $ApiMgmtContext
```

This command gets all of the APIs for the specified context.

### Example 2: Get an API by ID
```
PS C:\> Get-AzureRmApiManagementApi -Context $ApiMgmtContext -ApiId $ApiId
```

This command gets the API identified by the ID specified in the $ApiId variable.

### Example 3: Get an API by name
```
PS C:\> Get-AzureRmApiManagementApi -Context $ApiMgmtContext -Name "EchoApi"
```

This command gets the API named "EchoApi".

## PARAMETERS

### -ApiId
Specifies the ID of the API to get.

```yaml
Type: String
Parameter Sets: Find by ID
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Context
Specifies an **PsApiManagementContext** object that contains details about the context of the Azure API Management service.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the API to get.

```yaml
Type: String
Parameter Sets: Find by Name
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProductId
Specifies the ID of the product for which to get the API.

```yaml
Type: String
Parameter Sets: Find by product ID
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementContext

## OUTPUTS

### System.Collections.Generic.IList

## NOTES

## RELATED LINKS

[Export-AzureRmApiManagementApi](./Export-AzureRmApiManagementApi.md)

[Import-AzureRmApiManagementApi](./Import-AzureRmApiManagementApi.md)

[New-AzureRmApiManagementApi](./New-AzureRmApiManagementApi.md)

[Remove-AzureRmApiManagementApi](./Remove-AzureRmApiManagementApi.md)

[Set-AzureRmApiManagementApi](./Set-AzureRmApiManagementApi.md)
