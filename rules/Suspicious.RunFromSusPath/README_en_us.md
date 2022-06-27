



Contents
========

* [Suspicious.RunFromSusPath](#suspiciousrunfromsuspath)
	* [Suspicious.RunFromSusPath.A](#suspiciousrunfromsuspatha)
	* [Suspicious.RunFromSusPath.B](#suspiciousrunfromsuspathb)
	* [Suspicious.RunFromSusPath.C](#suspiciousrunfromsuspathc)
	* [Suspicious.RunFromSusPath.D](#suspiciousrunfromsuspathd)
	* [Suspicious.RunFromSusPath.E](#suspiciousrunfromsuspathe)

# Suspicious.RunFromSusPath

## Suspicious.RunFromSusPath.A
  
Status: Enabled

Behavioral Description:   
When the source process`*`initializes the following actions, HIPS module should let the user decide them.
- `Execute` the program under the path `*\Users\*\AppData\Roaming\>`
- `Execute` the program under the path `*\Users\*\AppData\>`
- `Execute` the program under the path `*\Users\>\>`
- `Execute` the program under the path `*\ProgramData\>`
- `Execute` the program under the path `*\Program Files\>`
- `Execute` the program under the path `*\Program Files (x86)\>`
- `Execute` the program under the path `*\Users\*\AppData\Local\>`
- `Execute` the program under the path `*\Users\>\Documents\>`
- `Execute` the program under the path `*\Users\>\Documents\>\>`
- `Read` the file under the path `*\Users\Public\>.bat`

## Suspicious.RunFromSusPath.B
  
Status: Enabled

Behavioral Description:   
When the source process`*`initializes the following actions, HIPS module should let the user decide them.
- `Execute` the program under the path `*\Recycler\*`
- `Execute` the program under the path `*\$RECYCLE.BIN\*`
- `Execute` the program under the path `*\System Volume Information\*`

## Suspicious.RunFromSusPath.C
  
Status: Disabled

Behavioral Description:   
When the source process`*`initializes the following actions, HIPS module should automatically block them.
- `Execute` the program under the path `*\ProgramData\>\>.exe`

## Suspicious.RunFromSusPath.D
  
Status: Enabled

Behavioral Description:   
When the source process`*\Windows\Sys?????\>`initializes the following actions, HIPS module should let the user decide them.
- `Execute` the program under the path `*\Users\*\AppData\Roaming\>\>.exe`

## Suspicious.RunFromSusPath.E
  
Status: Disabled

Behavioral Description:   
When the source process`*`initializes the following actions, HIPS module should automatically block them.
- `Execute` the program under the path `*\Users\*\AppData\Roaming\>\>.exe`
  
***rule.json hash: 3997ac4b56fb80d81d036c3beabcb423cfd73598afa0d93b5861c6523f10ac81***