# XeroRuby::Prepayment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **String** | See Prepayment Types | [optional] 
**contact** | [**Contact**](Contact.md) |  | [optional] 
**date** | **Date** | The date the prepayment is created YYYY-MM-DD | [optional] 
**status** | **String** | See Prepayment Status Codes | [optional] 
**line_amount_types** | [**LineAmountTypes**](LineAmountTypes.md) |  | [optional] 
**line_items** | [**Array&lt;LineItem&gt;**](LineItem.md) | See Prepayment Line Items | [optional] 
**sub_total** | **Float** | The subtotal of the prepayment excluding taxes | [optional] 
**total_tax** | **Float** | The total tax on the prepayment | [optional] 
**total** | **Float** | The total of the prepayment(subtotal + total tax) | [optional] 
**reference** | **String** | Returns Invoice number field. Reference field isn&#39;t available. | [optional] 
**updated_date_utc** | **DateTime** | UTC timestamp of last update to the prepayment | [optional] 
**currency_code** | [**CurrencyCode**](CurrencyCode.md) |  | [optional] 
**prepayment_id** | **String** | Xero generated unique identifier | [optional] 
**currency_rate** | **Float** | The currency rate for a multicurrency prepayment. If no rate is specified, the XE.com day rate is used | [optional] 
**remaining_credit** | **Float** | The remaining credit balance on the prepayment | [optional] 
**allocations** | [**Array&lt;Allocation&gt;**](Allocation.md) | See Allocations | [optional] 
**applied_amount** | **Float** | The amount of applied to an invoice | [optional] 
**has_attachments** | **Boolean** | boolean to indicate if a prepayment has an attachment | [optional] 
**attachments** | [**Array&lt;Attachment&gt;**](Attachment.md) | See Attachments | [optional] 

## Code Sample

```ruby
require 'XeroRuby'

instance = XeroRuby::Prepayment.new(type: null,
                                 contact: null,
                                 date: null,
                                 status: null,
                                 line_amount_types: null,
                                 line_items: null,
                                 sub_total: null,
                                 total_tax: null,
                                 total: null,
                                 reference: null,
                                 updated_date_utc: null,
                                 currency_code: null,
                                 prepayment_id: null,
                                 currency_rate: null,
                                 remaining_credit: null,
                                 allocations: null,
                                 applied_amount: 2.0,
                                 has_attachments: null,
                                 attachments: null)
```


