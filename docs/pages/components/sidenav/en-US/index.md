# Sidenav

An encapsulation of the Nav for the sidebar of the page.

- `<Sidenav>` Side navigation component.
- `<Sidenav.Header>` Navigates the header content.
- `<Sidenav.Body>` Navigation body content.

## Import

<!--{include:(components/sidenav/fragments/import.md)}-->

## Examples

### Default

<!--{include:`basic.md`}-->

### Appearance

`appearance` value include:`default`,`inverse`,`subtle`

> In high-contrast theme, all appearances looks the same as `default`.

<!--{include:`appearance.md`}-->

### Collapsed Menu

<!--{include:`collapsed.md`}-->

### Custom Side Navigation

- Set the `panel` property to customize a panel area.
- Set the `divider` property and set a split line.

<!--{include:`divider-panel.md`}-->

## Props

### `<Sidenav>`

| Property        | Type `(Default)`                                   | Description                                                |
| --------------- | -------------------------------------------------- | ---------------------------------------------------------- |
| appearance      | enum: 'default', 'inverse', 'subtle' `('default')` | Menu style                                                 |
| as              | ElementType `('div')`                              | You can use a custom element type for this component       |
| classPrefix     | string `('sidenav')`                               | The prefix of the component CSS class                      |
| defaultOpenKeys | string[]                                           | Open menu, corresponding to Dropdown eventkey              |
| expanded        | boolean `(true)`                                   | Whether to expand the Sidenav                              |
| onOpenChange    | (openKeys: string[], event) => void                | Menu opening callback function that changed                |
| openKeys        | string[]                                           | Open menu, corresponding to Dropdown eventkey (controlled) |
