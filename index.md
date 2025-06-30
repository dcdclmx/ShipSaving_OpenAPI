{% img src="./assets/banner.png" alt="Image description" withLightbox=true width="" height="" /%}

## Quick Start Guide
Welcome to the ShipSaving API
ShipSaving’s API offers a streamlined solution for integrating shipping capabilities directly into your application. With a single integration, you can access discounted rates from multiple carriers, create labels, track packages, schedule pickups, and more — all within one platform.

### This API allows you to:
- Create and manage orders
- Retrieve shipping rates
- Purchase and void shipping labels
- Generate SCAN forms for USPS and DHL
- Access account and carrier information


{% card title="📝 Record of Updates" %}
| Date       | Update                                                                 |
|------------|------------------------------------------------------------------------|
| 10/30/2024 | New API document                                                       |
| 10/30/2024 | Change to new endpoint                                                 |
| 10/30/2024 | Support check price list by Carrier Account                            |
| 10/30/2024 | Standardize and optimize error responses                               |
| 10/30/2024 | Add Get Account Balance interface                                      |
| 10/30/2024 | Add/Create/Get DHL eCommerce SCAN Form interfaces                      |
| 11/22/2024 | Add Get Carrier Account list interface                                 |
| 02/21/2025 | Add `label_type` param (PDF & PNG) to pricing-related APIs             |
| 02/21/2025 | Add 3 Canada Post service levels in Table 10                           |
| 06/17/2025 | Add GOFO_EXPRESS in Table 1                                            |
{% /card %}


###  API Integration Flow
#### 👍 Option 1:
1. Check Label Pricing List
2. Purchase Label

#### Option 2:
1. Directly Buy Label
💡 Limitation about this option: This interface is only applicable to you just have one same type carrier account, like one UPS account, one FEDEX account, one USPS account

#### Option 3 

1. Create Orders
2. Check Label Pricing List
3. Purchase Label

💡 Creating orders to our system is not required, you can keep your orders in your system


  



## Appendix
<details>
<summary>📦 Click to expand Carrier Service Types Table</summary>

| Carrier | Service Type |
|---------|---------------|
| USPS | usps_first_class_mail |
| USPS | usps_ground_advantage |
| USPS | usps_priority_mail |
| USPS | usps_priority_mail_express |
| USPS | usps_media_mail |
| USPS | usps_library_mail |
| USPS | usps_first_class_mail_international |
| USPS | usps_priority_mail_international |
| USPS | usps_priority_mail_express_international |
| UPS | ups_ground |
| UPS | ups_standard |
| UPS | ups_worldwide_saver |
| UPS | ups_worldwide_express |
| UPS | ups_worldwide_express_plus |
| UPS | ups_worldwide_expedited |
| UPS | ups_next_day_air |
| UPS | ups_next_day_air_saver |
| UPS | ups_next_day_air_early |
| UPS | ups_2nd_day_air |
| UPS | ups_2nd_day_air_am |
| UPS | ups_3_day_select |
| UPS | ups_surepost_less_than_1_lb |
| UPS | ups_surepost_1_lb_or_greater |
| UPS | ups_expedited_mail_innovations |
| UPS® Ground Saver | ups_surepost_1_lb_or_greater |
| FEDEX | fedex_ground |
| FEDEX | fedex_2_day |
| FEDEX | fedex_2_day_am |
| FEDEX | fedex_express_saver |
| FEDEX | fedex_standard_overnight |
| FEDEX | fedex_first_overnight |
| FEDEX | fedex_priority_overnight |
| FEDEX | fedex_international_economy |
| FEDEX | fedex_international_first |
| FEDEX | fedex_international_priority |
| FEDEX | fedex_home_delivery |
| FEDEX | fedex_smartpost |
| FEDEX | fedex_international_connect_plus |
| DHL_ECOMMERCE | dhl_ecommerce_parcel_expedited |
| DHL_ECOMMERCE | dhl_ecommerce_parcel_expedited_max |
| DHL_ECOMMERCE | dhl_ecommerce_parcel_ground |
| DHL_ECOMMERCE | dhl_ecommerce_bpm_expedited |
| DHL_ECOMMERCE | dhl_ecommerce_bpm_ground |
| DHL_ECOMMERCE | dhl_ecommerce_parcel_international_direct |
| DHL_ECOMMERCE | dhl_ecommerce_parcel_international_standard |
| DHL_ECOMMERCE | dhl_ecommerce_packet_international |
| DHL_EXPRESS | dhl_express_worldwide_b2c |
| DHL_EXPRESS | dhl_express_worldwide_b2c_nondoc |
| DHL_EXPRESS | dhl_express_jet_line_nondoc |
| DHL_EXPRESS | dhl_express_sprint_line |
| DHL_EXPRESS | dhl_express_euro_pack_doc |
| DHL_EXPRESS | dhl_express_break_bulk_express |
| DHL_EXPRESS | dhl_express_medical_express |
| DHL_EXPRESS | dhl_express_worldwide_doc |
| DHL_EXPRESS | dhl_express_0900_nondoc |
| DHL_EXPRESS | dhl_express_freight_worldwide_nondoc |
| DHL_EXPRESS | dhl_express_domestic_economy_select |
| DHL_EXPRESS | dhl_express_economy_select_nondoc |
| DHL_EXPRESS | dhl_express_domestic_express_0900 |
| DHL_EXPRESS | dhl_express_jumbo_box_nondoc |
| DHL_EXPRESS | dhl_express_0900 |
| DHL_EXPRESS | dhl_express_1030 |
| DHL_EXPRESS | dhl_express_1030_nondoc |
| DHL_EXPRESS | dhl_express_domestic_express |
| DHL_EXPRESS | dhl_express_domestic_express_1030 |
| DHL_EXPRESS | dhl_express_worldwide_nondoc |
| DHL_EXPRESS | dhl_express_medical_express_nodoc |
| DHL_EXPRESS | dhl_express_global_mail_business |
| DHL_EXPRESS | dhl_express_same_day |
| DHL_EXPRESS | dhl_express_1200_doc |
| DHL_EXPRESS | dhl_express_worldwide_ecx |
| DHL_EXPRESS | dhl_express_euro_pack_nondoc |
| DHL_EXPRESS | dhl_express_economy_select |
| DHL_EXPRESS | dhl_express_envelope |
| DHL_EXPRESS | dhl_express_1200_nondoc |
| DHL_EXPRESS | dhl_express_domestic_express_1200 |
| CANADA_POST | canada_post_priority |
| CANADA_POST | canada_post_expedited_parcel |
| CANADA_POST | canada_post_xpresspost |
| GOFO_EXPRESS | gofo_express_eco |

</details>

<details>
<summary>📦 Click to expand Predefined Carrier Packages Table</summary>

| Carrier | Package Type |
|---------|---------------|
| USPS | usps_postcard |
| USPS | usps_letter |
| USPS | usps_large_envelope_or_flat |
| USPS | usps_thick_envelope |
| USPS | usps_small_flat_rate_box |
| USPS | usps_medium_flat_rate_box |
| USPS | usps_large_flat_rate_box |
| USPS | usps_flat_rate_envelope |
| USPS | usps_padded_flat_rate_envelope |
| USPS | usps_legal_flat_rate_envelope |
| UPS | ups_letter |
| UPS | ups_25kg_box |
| UPS | ups_10kg_box |
| UPS | ups_tube |
| UPS | ups_pak |
| UPS | ups_express_box_small |
| UPS | ups_express_box_medium |
| UPS | ups_express_box_large |
| FEDEX | fedex_pak |
| FEDEX | fedex_tube |
| FEDEX | fedex_small_box |
| FEDEX | fedex_medium_box |
| FEDEX | fedex_large_box |
| FEDEX | fedex_extra_large_box |
| DHL_EXPRESS | dhl_express_jumbo_document |
| DHL_EXPRESS | dhl_express_jumbo_parcel |
| DHL_EXPRESS | dhl_express_document |
| DHL_EXPRESS | dhl_express_flyer |
| DHL_EXPRESS | dhl_express_domestic |
| DHL_EXPRESS | dhl_express_express_document |
| DHL_EXPRESS | dhl_express_envelope |
| DHL_EXPRESS | dhl_express_jumbo_box |
| DHL_EXPRESS | dhl_express_jumbo_junior_document |
| DHL_EXPRESS | dhl_express_junior_jumbo_box |
| DHL_EXPRESS | dhl_express_jumbo_junior_parcel |
| DHL_EXPRESS | dhl_express_other_dhl_packaging |
| DHL_EXPRESS | dhl_express_parcel |

</details>