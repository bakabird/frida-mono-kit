# frida-mono-kit

[NPM](https://www.npmjs.com/package/frida-mono-kit) | [GIT](https://github.com/bakabird/frida-mono-kit#readme)


> This lib develop base on https://github.com/freehuntx/frida-mono-api


This module is meant to be used inside of a frida module.  
An easy injector can be found here: [frida-inject](https://github.com/freehuntx/frida-inject)  
  
It will give you access to the mono c functions, exported by mono.  
For easy use, there are some helper methods you should check out.

## Note
The functions exposed by "MonoApi" are "ExNativefunctions".  
They have some more properties for easy use. See: [frida-ex-nativefunction](https://github.com/freehuntx/frida-ex-nativefunction)

## Example
### Using helper
```javascript
import { MonoApiHelper } from 'frida-mono-kit'

MonoApiHelper.AssemblyForeach(assembly => console.log(assembly))
```

### Using api
```javascript
import { MonoApi } from 'frida-mono-kit'

const domain = MonoApi.mono_domain_get()
```
