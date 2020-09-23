<div align="center">

## Hex & Decimal Conversion


</div>

### Description

Convert numbers from Hex to Decimal and from Decimal to Hex.
 
### More Info
 
Pass values to the functions:

Hex2Dec()

Dec2Hex()

Converted Hex/Decimal value..


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nick Radford](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nick-radford.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |
**Category**       |[Calculators & Science](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/calculators-science__2-71.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nick-radford-hex-decimal-conversion__2-2840/archive/master.zip)





### Source Code

```
<html>
<head>
<title>Hex & Decimal Conversion</title>
<script language="javascript">
<!--
function Hex2Dec(HexVal) {
	var HexVal = HexVal.toUpperCase();
	return parseInt(HexVal,16);
}
function Dec2Hex(DecVal) {
	var HexChars = '0123456789ABCDEF';
	var HexStr = ''
	while (DecVal>0){
		var HexStr = HexChars.charAt( DecVal%16 ) + HexStr;
		var DecVal = Math.floor(DecVal/16);
	}
	return HexStr
}
//-->
</script>
</head>
<body bgcolor="#ffffff">
<form name="ConvertIt">
	<table cellpadding="2" cellspacing="0" border="0">
	<tr>
		<td>Decimal Value</td>
		<td><input type="text" name="DecValue" size="10"></td>
		<td><input type="button" value="Convert to HEX" onclick="alert( Dec2Hex(document.ConvertIt.DecValue.value) )"></td>
	</tr>
	<tr>
		<td colspan="3">&nbsp;</td>
	</tr>
	<tr>
		<td>HEX Value</td>
		<td><input type="text" name="HexValue" size="10"></td>
		<td><input type="button" value="Convert to Decimal" onclick="alert( Hex2Dec(document.ConvertIt.HexValue.value) )"></td>
	</tr>
	</table>
</form>
</body>
</html>
```

