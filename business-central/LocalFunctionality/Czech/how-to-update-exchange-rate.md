---
title: Czech Local Functionality | Microsoft Docs
description: The following topics describe the local functionality in the Czech version of Business Central.
author: v-makune

ms-service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: CZ, Czech, Advance payment, Advance invoices, Payables, Finance,  Cash, EET, Cash Desk
ms.date: 12/30/2019
ms.reviewer: v-makune
ms.author: v-makune
---


# Exchange Rates Adjustment Feature

The majority of companies in the Czech Republic request the following improvements to be implemented in Exchange Rates Adjustment:

- Ability to run Exchange Rates Adjustment for Customers, Vendors and Bank Accounts separately
- Ability to have Exchange Rates Adjustment batch post adjustments in detail as well as summarized per currency
- Ability to run Exchange Rates Adjustment just as simulation (without posting) in Test Mode

On standard report Adjust Exchange Rates is now possible to:

- Set Bank Account, Customer, Vendor filter for adjustment
- Choose adjustment for Customer or Vendor or Bank Account
- Choose the test mode
- Choose summarizing entries
- Choose the method for dimension transfer

The Adjust Exchange Rate report feature also modifies the calculation principle for implemented gains and losses based on the Income Tax Act. This feature calculates the implemented gain or loss against the recently adjusted amount.

This feature in the standard version of Microsoft [!INCLUDE[d365fin](../../includes/d365fin_md.md)] reverses the non-implemented gain or loss first, and calculates the implemented gain or loss afterwards. The calculation is expressed against the amount in the initial exchange rate during the application of the payment and the invoice.

The new calculation principle is implemented for fluctuation in the already adjusted exchange rate.
The Adjust Exchange Rates batch job has been for Czech Advance Payments has also been extended.

# Exchange Rate Updating

The company is allowed to automatically update currency exchange rates using the exchange rate service.  

These have been improved by the ability to automatically update currency exchange rates from the CNB (Czech National Bank).  
The user can define the http service address and other exchange rate update parameters in the exchange rate service settings.


## VAT Exchange Rate

The exchange rate is located in documents, but Czech Republic requires the possibility to set different exchange rates for posting and VAT in sales and purchase documents. This feature adds the **VAT Currency Code** and **VAT Exchange Rate** fields in documents. Users can change the exchange rate for VAT before document posting.

## See Also

[Czech Local Functionality](czech-local-functionality.md)  
[Finance](../../finance.md)