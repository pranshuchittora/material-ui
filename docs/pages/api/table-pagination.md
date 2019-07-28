---
filename: /packages/material-ui/src/TablePagination/TablePagination.js
---

<!--- This documentation is automatically generated, do not try to edit it. -->

# TablePagination API

<p class="description">The API documentation of the TablePagination React component. Learn more about the props and the CSS customization points.</p>

```js
import { TablePagination } from '@material-ui/core';
```

A `TableCell` based component for placing inside `TableFooter` for pagination.

## Props

| Name | Type | Default | Description |
|:-----|:-----|:--------|:------------|
| <span class="prop-name">ActionsComponent</span> | <span class="prop-type">elementType</span> | <span class="prop-default">TablePaginationActions</span> | The component used for displaying the actions. Either a string to use a DOM element or a component. |
| <span class="prop-name">backIconButtonProps</span> | <span class="prop-type">object</span> |  | Props applied to the back arrow [`IconButton`](/api/icon-button/) component. |
| <span class="prop-name">classes</span> | <span class="prop-type">object</span> |  | Override or extend the styles applied to the component. See [CSS API](#css) below for more details. |
| <span class="prop-name">component</span> | <span class="prop-type">elementType</span> | <span class="prop-default">TableCell</span> | The component used for the root node. Either a string to use a DOM element or a component. |
| <span class="prop-name required">count&nbsp;*</span> | <span class="prop-type">number</span> |  | The total number of rows. |
| <span class="prop-name">labelDisplayedRows</span> | <span class="prop-type">func</span> | <span class="prop-default">({ from, to, count }) => `${from}-${to} of ${count}`</span> | Customize the displayed rows label. |
| <span class="prop-name">labelRowsPerPage</span> | <span class="prop-type">node</span> | <span class="prop-default">'Rows per page:'</span> | Customize the rows per page label. Invoked with a `{ from, to, count, page }` object. |
| <span class="prop-name">nextIconButtonProps</span> | <span class="prop-type">object</span> |  | Props applied to the next arrow [`IconButton`](/api/icon-button/) element. |
| <span class="prop-name required">onChangePage&nbsp;*</span> | <span class="prop-type">func</span> |  | Callback fired when the page is changed.<br><br>**Signature:**<br>`function(event: object, page: number) => void`<br>*event:* The event source of the callback<br>*page:* The page selected |
| <span class="prop-name">onChangeRowsPerPage</span> | <span class="prop-type">func</span> |  | Callback fired when the number of rows per page is changed.<br><br>**Signature:**<br>`function(event: object) => void`<br>*event:* The event source of the callback |
| <span class="prop-name required">page&nbsp;*</span> | <span class="prop-type">number</span> |  | The zero-based index of the current page. |
| <span class="prop-name required">rowsPerPage&nbsp;*</span> | <span class="prop-type">number</span> |  | The number of rows per page. |
| <span class="prop-name">rowsPerPageOptions</span> | <span class="prop-type">array</span> | <span class="prop-default">[10, 25, 50, 100]</span> | Customizes the options of the rows per page select field. If less than two options are available, no select field will be displayed. |
| <span class="prop-name">SelectProps</span> | <span class="prop-type">object</span> | <span class="prop-default">{}</span> | Props applied to the rows per page [`Select`](/api/select/) element. |

The `ref` is forwarded to the root element.

Any other props supplied will be provided to the root element ([TableCell](/api/table-cell/)).

## CSS

- Style sheet name: `MuiTablePagination`.
- Style sheet details:

| Rule name | Global class | Description |
|:-----|:-------------|:------------|
| <span class="prop-name">root</span> | <span class="prop-name">MuiTablePagination-root</span> | Styles applied to the root element.
| <span class="prop-name">toolbar</span> | <span class="prop-name">MuiTablePagination-toolbar</span> | Styles applied to the Toolbar component.
| <span class="prop-name">spacer</span> | <span class="prop-name">MuiTablePagination-spacer</span> | Styles applied to the spacer element.
| <span class="prop-name">caption</span> | <span class="prop-name">MuiTablePagination-caption</span> | Styles applied to the caption Typography components if `variant="caption"`.
| <span class="prop-name">selectRoot</span> | <span class="prop-name">MuiTablePagination-selectRoot</span> | Styles applied to the Select component root element.
| <span class="prop-name">select</span> | <span class="prop-name">MuiTablePagination-select</span> | Styles applied to the Select component `select` class.
| <span class="prop-name">selectIcon</span> | <span class="prop-name">MuiTablePagination-selectIcon</span> | Styles applied to the Select component `icon` class.
| <span class="prop-name">input</span> | <span class="prop-name">MuiTablePagination-input</span> | Styles applied to the `InputBase` component.
| <span class="prop-name">menuItem</span> | <span class="prop-name">MuiTablePagination-menuItem</span> | Styles applied to the MenuItem component.
| <span class="prop-name">actions</span> | <span class="prop-name">MuiTablePagination-actions</span> | Styles applied to the internal `TablePaginationActions` component.

You can override the style of the component thanks to one of these customizability points:

- With a rule name of the [`classes` object prop](/customization/components/#overriding-styles-with-classes).
- With a [global class name](/customization/components/#overriding-styles-with-global-class-names).
- With a theme and an [`overrides` property](/customization/globals/#css).

If it's not enough, you can find the [implementation of the component](https://github.com/mui-org/material-ui/blob/master/packages/material-ui/src/TablePagination/TablePagination.js) for more detail.

## Inheritance

The props of the [TableCell](/api/table-cell/) component are also available.
You can take advantage of this behavior to [target nested components](/guides/api/#spread).

## Notes

The component can cause issues in [StrictMode](https://reactjs.org/docs/strict-mode.html).

## Demos

- [Tables](/components/tables/)
