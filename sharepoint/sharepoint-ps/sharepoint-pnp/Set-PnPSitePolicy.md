---
external help file:
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/set-pnpsitepolicy
applicable: SharePoint Server 2013, SharePoint Server 2016, SharePoint Server 2019, SharePoint Online
schema: 2.0.0
---

# Set-PnPSitePolicy

## SYNOPSIS
Sets a site policy

## SYNTAX 

```powershell
Set-PnPSitePolicy -Name <String>
                  [-Web <WebPipeBind>]
                  [-Connection <SPOnlineConnection>]
```

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
Set-PnPSitePolicy -Name "Contoso HBI"
```

This applies a site policy with the name "Contoso HBI" to the current site. The policy needs to be available in the site.

## PARAMETERS

### -Name
The name of the site policy to apply

```yaml
Type: String
Parameter Sets: (All)

Required: True
Position: Named
Accept pipeline input: False
```

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: SPOnlineConnection
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

### -Web
This parameter allows you to optionally apply the cmdlet action to a subweb within the current web. In most situations this parameter is not required and you can connect to the subweb using Connect-PnPOnline instead. Specify the GUID, server relative url (i.e. /sites/team1) or web instance of the web to apply the command to. Omit this parameter to use the current web.

```yaml
Type: WebPipeBind
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)