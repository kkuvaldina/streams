# Badge

The `Badge` component creates a component that allows for basic information to be displayed.

Here is an example of what you’ll get out of the box:

![badge-example](badge-example.png)

```javascript
import BadgeComponent from 'badge.react';

<BadgeComponent
    imageAlt="Image of employee"
    imageSrc="/astro-panda-90x90.png"
    isModalHeader={ false }
    theme="newHire"
    title={ employeeData.fullName }
>
    <EmploymentSubtitles jobTitle={ employeeData.jobTitle } location="Cape Canaveral" />
</BadgeComponent>
```

Here are the properties it is looking for:

```javascript
{
    children,
    imageJSX,
    imageAlt = '',
    imageSrc = '',
    imageIcon = '',
    isModalHeader = true,
    theme,
    title = '',
    subTitle = '',
}
```
We leverage `children` here to allow for customization without cluttering the code. You can provide the basic details and a generic badge will be created or you can leverage children to customize the look of the data. `theme` allows you to tap into styles for a themed use. There are sub-components available for when the badge may have recurring usage. If you find yourself repeatedly adding a group of children create a component and give it a theme style if needed! `isModalHeader` styles the badge to look as if it is a modal header.

