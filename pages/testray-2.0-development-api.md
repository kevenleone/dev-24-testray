# Testray 2.0 - Development API's

TR2 is entirely created with React and Remote App, to have the best developer experience, we use some Headless API's and Liferay Global JS API

<div grid="~ cols-2 gap-2">
<div v-click>

#### Headless API's

<br />

- Headless Admin User
    - account
    - roles
    - user groups
- Headless Delivery
    - message board messages
    - message board threads
</div>
<div v-click>

#### Javascript API's

```ts
interface IThemeDisplay {
	getBCP47LanguageId(): () => string;
	getCompanyGroupId: () => number;
	getDefaultLanguageId: () => string;
	getLanguageId: () => string;
	getPathThemeImages: () => string;
	getScopeGroupId: () => number;
	getSiteGroupId: () => number;
	getUserId: () => string;
	getUserName: () => string;
}

interface ILiferay {
  authToken: string;
  ThemeDisplay: IThemeDisplay;
  Util: {
        openToast: (options?: any) => void;
    };
}
```

</div>
</div>
