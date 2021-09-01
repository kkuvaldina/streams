# Colored Icon

The `Colored Icon` component extends the usage of the fabric icon. Instead of being limited to brand colors or fabric gray10 you can now pass in any fabric named color (that aren’t themes at this time).

```javascript
import { ColoredIcon } from 'colored-icon';

<ColoredIcon
    classes="EmploymentSubtitles__subTitleIcon"
    fabricColorName="gray7"
    iconName="fab-employees-14x12"
/>
```

Here are the properties it is looking for:

```javascript
{
	classes?: string;
	fabricColorName: string;
	iconName: string;
}

```
The `classes` prop is to allow for hooks to do what you need with the icon. The `fabricColorName` must match one of the predefined fabric named colors as seen in the example. `iconName` must follow the same naming convention as fabric icon.

The component will return a `<span>` with the fabric icon inside. Inline styles are used to color the icon.
