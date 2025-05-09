.. _Enable the ECommerce Receipt Page:

##########################################
Enable the E-Commerce Service Receipt Page
##########################################

.. tags:: site operator

.. warning::
   This service is deprecated and was last tagged for the Redwood release. We are not fixing bugs or developing new features for it. For updates, `follow along on the DEPR ticket <https://github.com/openedx/public-engineering/issues/22>`_

The E-Commerce service includes a receipt page that you can display to users
after their orders are complete.

.. contents::
   :depth: 1
   :local:

.. _Enable the Receipt Page:

***********************
Enable the Receipt Page
***********************

To enable the default receipt page for the E-Commerce service, follow these
steps.

#. Sign in to the LMS Django administration console for your base URL. For
   example, ``http://{your_URL}/admin``.

#. On the **Site Administration** page, locate **Site_Configuration**.

#. In the **Site_Configuration** section, next to **Site configurations**,
   select **Change**.

#. On the **Change site configuration** page, locate the **Values** field, and
   then add the following JSON format value.

   ::

     {
      "ECOMMERCE_RECEIPT_PAGE_URL":"/checkout/receipt/?order_number="
      }

#. Select **Save**.



.. include:: /links.txt


**Maintenance chart**

+--------------+-------------------------------+----------------+------------------------------------+
| Review Date  | Working Group Reviewer        |   Release      |Test situation                      |
+--------------+-------------------------------+----------------+------------------------------------+
| 2025-03-09   | Sarina Canelake               | Sumac          | Deprecated                         |
+--------------+-------------------------------+----------------+------------------------------------+
