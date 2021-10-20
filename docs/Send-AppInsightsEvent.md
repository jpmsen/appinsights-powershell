---
external help file: AppInsights.dll-Help.xml
Module Name: AppInsights
online version:
schema: 2.0.0
---

# Send-AppInsightsEvent

## SYNOPSIS
PowerShell command used to track custom events in application insights.

## SYNTAX

```
Send-AppInsightsEvent -Name <String> [-Metrics <Hashtable>] [[-InstrumentationKey] <Guid>]
 [[-Properties] <Hashtable>] [-RoleName <String>] [-RoleInstance <String>] [<CommonParameters>]
```

## DESCRIPTION
PowerShell command used to track custom events in application insights.

## EXAMPLES

### Example 1
```powershell
Send-AppInsightsEvent -EventName "Apple Orderd" -Properties @{ "Fruit" = "Apple";  "Type" = "Granny Smith" } -Metrics @{ "Weight" = 12 }
```

## PARAMETERS

### -InstrumentationKey
The Application Insights Instrumentation Key.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Metrics
Optional dictionary with custom metrics.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Properties
Optional dictionary with custom properties.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleInstance
Defines whether the process was successfully processed.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleName
Defines whether the process was successfully processed.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The Event that is transmitted.

```yaml
Type: String
Parameter Sets: (All)
Aliases: EventName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## NOTES

## RELATED LINKS