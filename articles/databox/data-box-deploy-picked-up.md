---
title: Tutorial to ship Azure Data Box back| Microsoft Docs
description: In this tutorial, learn how to return Azure Data Box, including preparing to ship, shipping Data Box, verifying data upload, and erasing data from Data Box.
services: databox
author: alkohli

ms.service: databox
ms.subservice: pod
ms.topic: tutorial
ms.date: 10/17/2021
ms.author: alkohli
ms.localizationpriority: high

# Customer intent: As an IT admin, I need to be able to return a Data Box to upload on-premises data from my server onto Azure.
---

::: zone target="docs"

# Tutorial: Return Azure Data Box and verify data upload to Azure

::: zone-end

::: zone target="chromeless"

## Return Data Box and verify data upload to Azure

::: zone-end

::: zone target="docs"

This tutorial describes how to return Azure Data Box and verify the data uploaded to Azure.

In this tutorial, you will learn about topics such as:

> [!div class="checklist"]
>
> * Prerequisites
> * Prepare to ship
> * Ship Data Box to Microsoft
> * Verify data upload to Azure
> * Erasure of data from Data Box

## Prerequisites

Before you begin, make sure:

* You've have completed the [Tutorial: Copy data to Azure Data Box and verify](data-box-deploy-copy-data.md).
* Copy jobs are complete and there are no errors on the **Connect and copy** page. **Prepare to ship** can't run if copy jobs are in progress or there are errors in the **Connect and copy** page.

## Prepare to ship

[!INCLUDE [data-box-prepare-to-ship](../../includes/data-box-prepare-to-ship.md)]

::: zone-end

::: zone target="chromeless"

After the data copy is complete, you prepare and ship the device. When the device reaches Azure datacenter, data is automatically uploaded to Azure.

## Prepare to ship

Before you prepare to ship, make sure that copy jobs are complete.

1. Go to **Prepare to ship** page in the local web UI and start the ship preparation.
2. Turn off the device from the local web UI. Remove the cables from the device.

The next steps are determined by where you're returning the device.

::: zone-end

::: zone target="docs"

## Ship Data Box back

Make sure the data copy to the device completed and the **Prepare to ship** run was successful. Based on the region where you're shipping the device, the procedure is different.

### Microsoft managed shipping

Follow the guidelines for the region you're shipping from if you're using Microsoft managed shipping.

::: zone-end

## [US & Canada](#tab/in-us-canada)

Take the following steps if returning the device in US or Canada.

1. Make sure that the device is powered off and cables are removed.
2. Spool and securely place the power cord that was provided with device in the back of the device.
3. Ensure that the shipping label is displayed on the E-ink display and schedule a pickup with your carrier. If the label is damaged or lost or not displayed on the E-ink display, contact Microsoft Support. If the Support suggests, then you can go to **Overview > Download shipping label** in the Azure portal. Download the shipping label and affix on the device. 
4. Schedule a pickup with UPS if returning the device. To schedule a pickup:

    * Call the local UPS (country/region-specific toll free number).
    * In your call, quote the reverse shipment tracking number as shown in the E-ink display or your printed label. If you don't quote the tracking number, UPS will require an additional charge during pickup.
    * If any issues come up while you're scheduling a pickup, or you're asked to pay additional fees, contact Azure Data Box Operations. Send email to [adbops@microsoft.com](mailto:adbops@microsoft.com).

    Instead of scheduling the pickup, you can also drop off the Data Box at the nearest drop-off location.
4. Once the Data Box is picked up and scanned by your carrier, the order status in the portal updates to **Picked up**. A tracking ID is also displayed.

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box

Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

## [Europe](#tab/in-europe)

Take the following steps if you're returning the device in Europe.

1. Make sure that the device is powered off and cables are removed.
2. Spool and securely place the power cord that was provided with device in the back of the device.
3. Ensure that the shipping label is displayed on the E-ink display and schedule a pickup with your carrier. If the label is damaged or lost or not displayed on the E-ink display, contact Microsoft Support. If the Support suggests, then you can go to **Overview > Download shipping label** in the Azure portal. Download the shipping label and affix on the device.
1. **If you're shipping from Germany or Switzerland,** the Azure datacenter requires advance notice of all device returns:
    1. Email Azure Data Box Operations, using the following template, to receive an Inbound ID. Send email to [adbops@microsoft.com](mailto:adbops@microsoft.com).

       ```
       To: adbops@microsoft.com
       Subject: Request for Azure Data Box Inbound ID: <orderName> 
       Body: 
        
       I am ready to return an Azure Data Box and would like to request an Inbound ID for the following order:
       
       Order Name: <orderName>
       Return Tracking Number: <returnTracking#>
       ```

    1. Write down the Inbound ID number provided by Azure Data Box Operations, and paste it onto the unit, where it is clearly visible, near the return label.
1. Schedule a pickup with UPS if returning the device. To schedule a pickup:

    * Call the local UPS (country/region-specific toll free number).
    * In your call, quote the reverse shipment tracking number as shown in the E-ink display or your printed label. If you don't quote the tracking number, UPS will require an additional charge during pickup.
    * If any issues come up while you're scheduling a pickup, or you're asked to pay additional fees, contact Azure Data Box Operations. Send email to [adbops@microsoft.com](mailto:adbops@microsoft.com).

    Instead of scheduling the pickup, you can also drop off the Data Box at the nearest drop-off location.

    **If you're shipping from Germany or Switzerland,** you can also [use self-managed shipping](data-box-deploy-picked-up.md#self-managed-shipping).

4. Once the Data Box is picked up and scanned by your carrier, the order status in the portal updates to **Picked up**. A tracking ID is also displayed.


::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box

Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

## [Australia](#tab/in-australia)

Azure datacenters in Australia have an additional security notification. All the inbound shipments must have an advanced notification. Take the following steps to ship in Australia.

1. Keep the original box used to ship the device for return shipment.
2. Make sure that the data copy to device is complete and **Prepare to ship run** is successful.
3. Power off the device and remove the cables.
4. Spool and securely place the power cord that was provided with the device in the back of the device.
5. Book a pickup online at the [DHL Link](https://mydhl.express.dhl/au/en/schedule-pickup.html#/schedule-pickup#label-reference).

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box

Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

## [Japan](#tab/in-japan)

1. Keep the original box used to ship the device for return shipment.
2. Power off the device and remove the cables.
3. Spool and securely place the power cord that was provided with the device in the back of the device.
4. Write your company name and address information on the consignment note as your sender information.
5. Email Quantium Solutions using the following email template.

    * If Japan Post Chakubarai consignment note wasn't included or is missing, note that in this email. Quantium Solutions Japan will request Japan Post to bring the consignment note upon pickup.
    * If you have multiple orders, email to ensure individual pickup.

    ```
    To: Customerservice.JP@quantiumsolutions.com
    Subject: Pickup request for Azure Data Box｜Job name： 
    Body:
    - Japan Post Yu-Pack tracking number (reference number)：
    - Requested pickup date：mmdd (Select a requested time slot from below).
    a. 08：00-13：00 
    b. 13：00-15：00 
    c. 15：00-17：00 
    d. 17：00-19：00 
    ```

6. Receive an email confirmation from Quantium Solutions after you've booked a pickup. The email confirmation also includes information on the Chakubarai consignment note.

If needed, you can contact Quantium Solutions Support (Japanese language) at the following information:

* Email：Customerservice.JP@quantiumsolutions.com 
* Telephone：03-5755-0150 

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box
 
Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

## [Singapore](#tab/in-singapore)

1. Keep the original box used to ship the device for return shipment.
2. Note down the tracking number (shown as reference number on the **Prepare to Ship** page of the Data Box local web UI). The tracking number is available after the **Prepare to ship** step completes successfully. Download the shipping label from this page and paste on the packing box.
3. Power off the device and remove the cables.
4. Spool and securely place the power cord that was provided with the device in the back of the device. 
5. Email SingPost Customer Service using the following email template with the tracking number.

    ```
    To: kadcustcare@singpost.com
    Subject: Microsoft Azure Pickup - OrderName 
    Body: 
        1. Requestor name  
        2. Requestor contact number
        3. Requestor collection address
        4. Preferred collection date
    ```

   > [!NOTE]
   > For booking requests received on a business day:
   > * Before 3 PM, pickup will be the next business day between 9 AM and 1 PM.
   > * After 3 PM, pickup will be the next business day between 2 PM to 6 PM.  

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box

Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

## [South Africa](#tab/in-sa)

1. Pack the device for return shipment in the original box.
2. Spool and securely place the power cord that was provided with the device in the back of the device.
3. Note the tracking number (shown as reference number on the **Prepare to Ship** page of the Data Box local web UI). The tracking number is available after the "Prepare to ship" step completes successfully. Download the shipping label from this page, and paste it on the packing box.
4. Request a return code from Azure Data Box Operations. A return code is required for delivering the package back to the datacenter. Send email to [adbops@microsoft.com](mailto:adbops@microsoft.com). Note this code on the shipping label next to the return address, where it is clearly visible.
5. Book a pickup with DHL using one of the following methods:
 
   * Book a pickup online by going to [DHL Express South Africa, **Schedule a Pickup**](https://mydhl.express.dhl/za/en/schedule-pickup.html#/schedule-pickup#label-reference).
   * Send an email to [Priority.Support@dhl.com](mailto:Priority.Support@dhl.com) using the following template:

     ```output
     To: Priority.Support@dhl.com
     Subject: Pickup request for Microsoft Azure
     Body: Need pick up for the below shipment
       *  DHL tracking number: (reference number/waybill number)
       *  Requested pickup date: yyyy/mm/dd;time:HH MM
       *  Shipper contact: (company name)
       *  Contact person: 
       *  Phone number: 
       *  Full physical address: 
       *  Item to be collected: Azure Dt
     ```

    * Or drop off the package at the nearest DHL service point.

6. If you come across any issues, email [Priority.Support@dhl.com](mailto:Priority.Support@dhl.com) with details of the issue(s), and put the waybill number in the Subject: line. You can also call +27(0)119213902.

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box

Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

## [Hong Kong](#tab/in-hk)

1. Pack the device for return shipment in the original box.
2. Spool and securely place the power cord that was provided with the device in the back of the device.
3. Call the **Quantium Solutions** hotline at **(852) 2318 1213** during office hours (9am to 6pm, Monday to Friday).  
4. Quote Microsoft Azure pickup and the reference number and tracking number (above barcode) on the return shipping label to arrange for a collection.
5. You'll get a verbal confirmation of the pickup schedule. If the courier doesn't arrive for collection, call the Quantium Solutions hotline for alternate arrangements.
6. Upon booking a pickup with Quantium Solutions, share the confirmation with [Microsoft Data Box Operations Asia](mailto:adbo@microsoft.com) using the following template:

    ```output
    To: adbo@microsoft.com
    Subject: Microsoft Data Box Job: [order name] has completed copy
    Body:
    We have confirmed the pickup details with Quantium Solutions.

       * Requestor name:
       * Requestor contact number:
       * Pickup Date:  
       * Pickup time:
    ```

If you come across any issues, email Data Box Operations Asia [adbo@microsoft.com](mailto:adbo@microsoft.com) with details of the issue(s), and put the job name in the Subject: line.

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box
 

::: zone-end

## [UAE](#tab/in-uae)

1. Keep the original box used to ship the device for return shipment.
2. Make sure the data copy to device is complete, and the **Prepare to ship** step completed successfully.
3. Note the reference number on the **Prepare to ship** page of the device local web UI.
4. Power off the device, and remove the cables. Spool and securely place the power cord that was provided with the device in the back of the device.
6. Pack the device for return shipment in the original box.
7. Email [Azure Data Box Operations](mailto:adbops@microsoft.com) to get an ID that will be used to identify the package when it arrives back at the datacenter.
8. Write down this ID on the printed shipping label, next to the return address so that it’s clearly visible.  
9. Book a pickup online by going to [DHL Express UAE](https://mydhl.express.dhl/ae/en/home.html#/schedulePickupTab) > **Schedule a Pickup**.
   - Enter the reference number from the **Prepare to ship** page of the device local web UI in the waybill number field.
   - Bookings are accepted from 9:00 AM – 2:00 PM six days a week (excluding Fri and public holidays).
   - Pickup requests should be placed at least 90 minutes before customer closing time.
10. If you come across any issue with the DHL booking tool, you can contact DHL using any of these methods:
    - Call 04-2924545.
    - Email [ecom.ae@dhl.com](mailto:ecom.ae@dhl.com) with details of the issue(s), and put the waybill number in the Subject: line.
    - Call DHL Customer Support at 600 567567.

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box
 
Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

<!--## [In Korea](#tab/in-korea) 

1. Retain the original box used to ship the device for return shipment.
2. Note down the tracking number (shown as reference number on the **Prepare to Ship** page of the Data Box local web UI). The tracking number is available after the **Prepare to ship** step successfully completes. Download the shipping label from this page and paste on the packing box. 
3. Power off the device and remove the cables.
4. Spool and securely place the power cord that was provided with the device in the back of the device. 

Request pickup  
If consignment note is present:  

1. Call Quantium Solutions International hotline at 070-8231-1418 during office hours (10 AM to 5 PM, Monday to Friday). Quote Microsoft Azure pickup and the service request number to arrange for a collection.
2. If the hotline is busy, email microsoft@rocketparcel.com, with the email subject Microsoft Azure Pickup and the service request number as reference.  
3. If the courier does not arrive for collection, call Quantium Solutions International hotline for alternate arrangements.  
4. You will receive an email confirmation for the pickup schedule.  

Exception process
If the consignment note is not present:
1. Call Quantium Solutions International hotline at 070-8231-1418 during office hours (10 AM to 5 PM, Monday to Friday). Quote Microsoft Azure pickup and the service request number. Specify that you need a new consignment note to arrange for a collection. Provide sender (customer), receiver information (Azure datacenter), and reference number (service request number).
2. If the hotline is busy, email microsoft@rocketparcel.com, with the email subject Microsoft Azure Pickup and the service request number as reference.
3. If the courier does not arrive for collection, call Quantium Solutions International hotline for alternate arrangements.
4. You get a verbal confirmation if request is made via telephone.  
::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box
 
Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

::: zone target="docs"

[!INCLUDE [data-box-verify-upload-return](../../includes/data-box-verify-upload.md)]

::: zone-end
-->

---

### Self-managed shipping

Follow the guidelines for the region you're shipping from if you're using Microsoft managed shipping.

If you're using Data Box in US Government, Japan, Singapore, Korea, India, South Africa, United Kingdom, Germany, Switzerland, West Europe, Australia, or Brazil, and you selected self-managed shipping when you created your order, follow these instructions.

1. Write down the Authorization code that's shown on the **Prepare to Ship** page of the local web UI for the Data Box after the step completes successfully.
2. Power off the device and remove the cables. Spool and securely place the power cord that was provided with the device at the back of the device.
3. When you're ready to return the device, send an email to the Azure Data Box Operations team using the template below.

    ```
    To: adbops@microsoft.com
    Subject: Request for Azure Data Box drop-off for order: 'orderName'
    Body:
        1. Order name  
        2. Authorization code available after Prepare to Ship has completed [Yes/No]  
        3. Contact name of the person dropping off. You will need to display a government-approved ID during the drop off.
    ```

   > [!NOTE]
   > - Required information for return may vary by region. 
   > - If you're returning a Data Box in Brazil, see [Use self-managed shipping for Azure Data Box](data-box-portal-customer-managed-shipping.md) for detailed instructions. 

::: zone target="chromeless"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload](../../includes/data-box-verify-upload.md)]

## Erasure of data from Data Box
 
Once the upload to Azure is complete, the Data Box erases the data on its disks as per the [NIST SP 800-88 Revision 1 guidelines](https://csrc.nist.gov/News/2014/Released-SP-800-88-Revision-1,-Guidelines-for-Medi).

::: zone-end

---

::: zone target="docs"

## Verify data upload to Azure

[!INCLUDE [data-box-verify-upload-return](../../includes/data-box-verify-upload-return.md)]

::: zone-end
