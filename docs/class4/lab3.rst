Lab 3: API Protection
=====================================

add description.

**Scenario**

A Social Security Number (SSN) has been detected within the response body of the "getbydob"
endpoint. This is a misconfiguration in the API, which isn’t approved for this Data Type based
on its Data Classification. 

Take action to block usage of the "getbydob" endpoint until misconfiguration is resolved. 

**Expected Lab Time: ?? minutes**

Task 1: Simulate...
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Add Description

#. Add more steps.

   .. image:: _static/update_image.png
      :width: 800px

Task 2: Attaching API Protection to Load Balancer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In this task's series of steps you will enable the API Protection feature on the
previously built Load Balancer object delivering the targeted API.

#. In the left-hand navigation of the **Web App & API Protection** service, click on **Load Balancers > HTTP Load**
   **Balancers** under the **Manage** section.

   .. image:: _static/update_image.png
      :width: 800px

#. In the resulting **Load Balancers** window, click on the three dots **...** in the
   **Action** column, and the select **Manage Configuration**.

   .. image:: _static/update_image.png
      :width: 800px

#. Click **Edit Configuration** in the top-right corner.

   .. image:: _static/update_image.png
      :width: 800px

#. In the **API Protection > API Protection Rules** section, click the **Configure** link.

   .. image:: _static/update_image.png
      :width: 800px

#. In the resulting **API Protection Rules** window, click **Configure** in the
   **API Endpoints** section.

   .. image:: _static/update_image.png
      :width: 800px

#. Click **Add Item** in the **API Endpoints** window.

   .. image:: _static/update_image.png
      :width: 800px

#. In the resulting window, input **block-endpoint** in the **Name** field of the
   **Metadata** section.

#. In the **Action** area, click the drop-down arrow indicated and select **Deny**.

   .. image:: _static/update_image.png
      :width: 800px

#. In the **API Endpoint** section, click on the **API Endpoint** input field as indicated.

#. Select the **See Suggestions** link.

   .. image:: _static/update_image.png
      :width: 800px

#. Select **/api/customerlookup/getbydob** from the available options provided.

   .. note::
      *The available endpoints are provided by the swagger previously imported,
      or identified by API Discovery*

#. In the **HTTP Methods** area, click in the **Method List** input field.

   .. image:: _static/update_image.png
      :width: 800px

#. Select **Any** from the available methods provided.

   .. note::
      *Multiple methods can be selected if needed*

   .. image:: _static/update_image.png
      :width: 800px

#. Review the configuration and click, the **Apply** button.

   .. image:: _static/update_image.png
      :width: 800px

#. Review the API Endpoint deny rule and click, the **Apply** button.

   .. image:: _static/update_image.png
      :width: 800px

#. Note that API Protection Rules are configure for the API Endpoints and click, the
   **Apply** button.

   .. image:: _static/update_image.png
      :width: 800px

#. Select **Other Settings** on the left then click on **Save and Exit**
   at the bottom right of window.

   .. image:: _static/update_image.png
      :width: 800px

Task 3: Simulate...
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Add Description

#. Add more steps.

   .. image:: _static/update_image.png
      :width: 800px

**End of Lab**

.. image:: _static/update_image.png
   :width: 800px
