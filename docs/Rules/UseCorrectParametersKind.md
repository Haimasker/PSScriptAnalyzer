# UseCorrectParametersKind

**Severity Level: Warning**

## Description

All functions should have same parameters definition kind specified in the rule. Either using inline parameters in function definition or using param() block inside function body.

## How to Fix

Rewrite function so it defines parameters as specified in the rule

## Example

### Correct for parameters definition kind set to 'Inline':
``````PowerShell
function f([Parameter()]$FirstParam) {
    return
}
``````

### Correct for parameters definition kind set to 'ParamBlock':
``````PowerShell
function f {
    param([Parameter()]$FirstParam)
    return
}
``````