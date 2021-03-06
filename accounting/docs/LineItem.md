# XeroRuby::LineItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**line_item_id** | **String** | LineItem unique ID | [optional] 
**description** | **String** | Description needs to be at least 1 char long. A line item with just a description (i.e no unit amount or quantity) can be created by specifying just a &lt;Description&gt; element that contains at least 1 character | [optional] 
**quantity** | **Float** | LineItem Quantity | [optional] 
**unit_amount** | **Float** | LineItem Unit Amount | [optional] 
**item_code** | **String** | See Items | [optional] 
**account_code** | **String** | See Accounts | [optional] 
**tax_type** | **String** | The tax type from TaxRates | [optional] 
**tax_amount** | **Float** | The tax amount is auto calculated as a percentage of the line amount (see below) based on the tax rate. This value can be overriden if the calculated &lt;TaxAmount&gt; is not correct. | [optional] 
**line_amount** | **Float** | If you wish to omit either of the &lt;Quantity&gt; or &lt;UnitAmount&gt; you can provide a LineAmount and Xero will calculate the missing amount for you. The line amount reflects the discounted price if a DiscountRate has been used . i.e LineAmount &#x3D; Quantity * Unit Amount * ((100 – DiscountRate)/100) | [optional] 
**tracking** | [**Array&lt;LineItemTracking&gt;**](LineItemTracking.md) | Optional Tracking Category – see Tracking.  Any LineItem can have a  maximum of 2 &lt;TrackingCategory&gt; elements. | [optional] 
**discount_rate** | **Float** | Percentage discount being applied to a line item (only supported on  ACCREC invoices – ACC PAY invoices and credit notes in Xero do not support discounts | [optional] 
**discount_amount** | **Float** | Discount amount being applied to a line item. Only supported on ACCREC invoices - ACCPAY invoices and credit notes in Xero do not support discounts. | [optional] 
**repeating_invoice_id** | **String** | The Xero identifier for a Repeating Invoice | [optional] 

## Code Sample

```ruby
require 'XeroRuby'

instance = XeroRuby::LineItem.new(line_item_id: 00000000-0000-0000-0000-000000000000,
                                 description: null,
                                 quantity: null,
                                 unit_amount: null,
                                 item_code: null,
                                 account_code: null,
                                 tax_type: null,
                                 tax_amount: null,
                                 line_amount: null,
                                 tracking: null,
                                 discount_rate: null,
                                 discount_amount: null,
                                 repeating_invoice_id: 00000000-0000-0000-0000-000000000000)
```


