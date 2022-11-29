---
title: Remote App Configuration
---

# Remote App Configuration

To start developement with Vite and hot reload is necessary to change the links of chunk, in remote app configuration of Liferay Portal

<div grid="~ cols-2 gap-3">

<img m="t-5" border="rounded" src="assets/remot_app_configuration.png" />
<div>

##### refresh.ts

```ts
import RefreshRuntime from '/@react-refresh';

RefreshRuntime.injectIntoGlobalHook(window);
window.$RefreshReg$ = () => {};
window.$RefreshSig$ = () => (type) => type;

window.__vite_plugin_react_preamble_installed__ = true;

declare global {
	interface Window {
		$RefreshReg$: () => void;
		$RefreshSig$: () => (type: string) => string;
		__vite_plugin_react_preamble_installed__: boolean;
	}
}
```
</div>

</div>


<style>
   .line {
      font-size: 10px;
   }
</style>

<!--
hello everyone, great to be here with you all, so I'll explain a little bit about our development process.

As keven mentioned before, we are using the remote app to develop Testray 2.

to make the development go faster we used vite which gave us the possibility to use hot realoading.
-->
