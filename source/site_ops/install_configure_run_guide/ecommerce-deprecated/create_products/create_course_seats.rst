.. _Create Course Seats:

####################
Create Course Seats
####################

.. tags:: site operator

.. warning::
   This service is deprecated and was last tagged for the Redwood release. We are not fixing bugs or developing new features for it. For updates, `follow along on the DEPR ticket <https://github.com/openedx/public-engineering/issues/22>`_

A course seat represents an enrollment track, sometimes called an enrollment
mode. For information about the enrollment tracks that edX offers, see
:term:`Enrollment track`.

You create course seats by creating a course on the **Create New Course** page
in the E-Commerce Course Administration tool, which is located at
``http://localhost:8002/courses/``. After you create a course, the E-Commerce
service creates the course seats that are associated with that course.

To create a course seat, follow these steps.

#. Start the E-Commerce Service on your site. For details, see :ref:`Start
   ECommerce Service`.

#. In a browser on your E-Commerce server, go to
   ``http://localhost:8002/courses/`` to access the E-Commerce Course
   Administration tool.

#. On the **Courses** page, select **Add New Course**.

#. On the **Create New Course** page, enter the following information for your
   course.

   * Course ID
   * Course Name
   * Course Type
   * Course Seats
   * Bulk :ref:`Enrollment Code<Enable and Create Enrollment Codes>` Yes/No

   For **Course Type**, select a course type and the options for that course
   type.

     * If you select **Free (Audit)**, you must specify whether you want to
       allow honor code learners to earn an honor code certificate. To do this,
       select **Yes** under **Include Honor Seat**.

     * If you select **Verified**, you must add the following information.

       * **Price (in USD)**
       * **Upgrade Deadline**
       * **Verification Deadline**
       * **Include Honor Seat**: This option grants honor code certificates to
         learners who successfully complete the course.

     * If you select **Professional Education**, you must add the following
       information.

       * **Price (in USD)**
       * **ID Verification Required?**
       * **Upgrade Deadline**

       * **Verification Deadline**: This option is required if you select
         **Yes** for **ID Verification Required?**

     * If you select **Credit**, you must add the following information.

       * **Price (in USD)**: The price for a verified certificate.
       * **Upgrade Deadline**
       * **Credit Provider**
       * **Price (USD)**: The price for course credit.
       * **Credit Hours**
       * **Upgrade Deadline**
       * **Verification Deadline**
       * **Include Honor Seat**: This option grants honor code certificates to
         learners who successfully complete the course.
         

#. Select **Create Course**.

.. include:: /links.txt


**Maintenance chart**

+--------------+-------------------------------+----------------+------------------------------------+
| Review Date  | Working Group Reviewer        |   Release      |Test situation                      |
+--------------+-------------------------------+----------------+------------------------------------+
| 2025-03-09   | Sarina Canelake               | Sumac          | Deprecated                         |
+--------------+-------------------------------+----------------+------------------------------------+
