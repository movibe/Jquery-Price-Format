# JQuery Price Format

jQuery Price Format Plugin is a plugin to format input text fields as prices. For example, if you type 123456, the plugin updates it to US$ 1,234.56. It is costumizable, so you can use other prefixes and separators (for example, use it to get R$ 1.234,55).

## Examples

### Basic Usage
`$('#your-input-here').priceFormat();`

### Customize

`$('#your-input-here').priceFormat({
    prefix: 'R$ ',
    centsSeparator: ',',
    thousandsSeparator: '.'
`});`

### Skipping some option
`$('#example3').priceFormat({
    prefix: '',
    thousandsSeparator: ''
});`

### Working with limits
`$('#example4').priceFormat({
    limit: 5,
    centsLimit: 3
});`

### Clear Prefix on Blur
`$('#example5').priceFormat({
    clearPrefix: true
});`

### Allow Negatives
`$('#example6').priceFormat({
    allowNegative: true
});`





