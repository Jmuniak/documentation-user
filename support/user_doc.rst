.. :banner: banners/support.jpg


===============================
Contribute to the documentation
===============================

First of all...
===============

**... Thank you for landing here and helping us to improve the user documentation of Odoo.**


Edit an existing page
=====================

0. As our documentation is maintained on GitHub, you'll need a free `GitHub account <https://help.github.com/en/articles/signing-up-for-a-new-github-account>`_.
1. Pick a page in our `user documentation <https://www.odoo.com/documentation/user>`_. **Please take care of choosing the right version of Odoo.**
2. Click on **Edit on Github** in the left menu.

   .. image:: ./media/edit_on_github.png
       :align: center
       :alt: Click on "Edit on Github".

3. If this is the first time you edit our documentation, click on **Fork repository**, else you won't see this step.
4. Use Github's editor to add your text. Text is tagged with a simple syntax called `RST <http://docutils.sourceforge.net/rst.html>`_. Don't worry, it's not so hard to learn 🤓... See the following section of this document for a quick overview of RST commands.

   .. image:: ./media/add_text.png
       :align: center
       :alt: Use Github's editor to add your text.

5. Click on **Preview changes** to review your contribution in a human-readable format.

   .. image:: ./media/preview_changes.png
       :align: center
       :alt: Click on "Preview changes" to review your contribution.

6. In the **Propose file change** section, add a short title to your contribution. The title should summarize your changes. You may use the second box to add an extended description if your contribution requires a longer explanation.

   .. image:: ./media/propose_changes.png
       :align: center
       :alt: Add a title and submit your contribution.

7. Submit your contribution by clicking on **Propose file change**.
8. Click on **Create pull request**.
9. Wait for an Odoo maintainer to add your contribution. Thank you for your help!

.. warning::
    There is no automatic port of your edit to another version of the documentation.

    If your change should apply to multiple versions of Odoo, please warn us in your contribution message.


RST Cheat Sheet
---------------

Here is a summary of the markup elements you may use while editing our documentation.

+------------------------------+--------------------------+---------------------------------------+
| Code                         | Display                  | Comments                              |
+==============================+==========================+=======================================+
| .. code-block:: rst          | Text in *italics*        |                                       |
|                              |                          |                                       |
|     Text in *italics*        |                          |                                       |
+------------------------------+--------------------------+---------------------------------------+
| .. code-block:: rst          | Text in **bold** letters |                                       |
|                              |                          |                                       |
|     Text in **bold** letters |                          |                                       |
+------------------------------+--------------------------+---------------------------------------+
| .. code-block:: rst          | 1. Numbered              | Must be surrounded by white lines.    |
|                              | 2. Bullet                |                                       |
|    1. Numbered               | 3. List                  |                                       |
|    2. Bullet                 |                          |                                       |
|    3. List                   |                          |                                       |
+------------------------------+--------------------------+---------------------------------------+
| .. code-block:: rst          | - Numbered               | Must be surrounded by white lines.    |
|                              | - Bullet                 |                                       |
|    - Bullet                  | - List                   |                                       |
|    - Point                   |                          |                                       |
|    - List                    |                          |                                       |
+------------------------------+--------------------------+---------------------------------------+
| .. code-block:: rst          | This is `a  hyper link   | - Here is `how to enter backticks     |
|                              | <https://www.odoo.com>`_.|   on your keyboard                    |
|    This is `a hyper link     |                          |   <https://superuser.com/a/254077>`_. |
|    <https://www.odoo.com>`_. |                          | - Don't forget terminal *underscore*. |
+------------------------------+--------------------------+---------------------------------------+


.. note::
    There are many more commands available, see `comprehensive documentation <http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html>`_ of RST.


Add images to your documents
============================


.. warning::
    This procedure is possible only for users who have **push** access on the documentation repository (eg: mainly, Odoo maintainers).
    We are working on improving this.

1. First of all, prepare your screenshots.

   - They must be good-quality PNG images.
   - Crop your screenshots to display only the relevant part of the screen. Large screenshots are hard
     to read and don't display well in a documentation.
   - Always take your screenshots on a demo instance of Odoo; **never** include any personal data.

2. Upload them to the ``media/`` directory which is located next to the page you are editing. If the directory does not exist, create it.
3. When editing your page, use this code piece in order to load your image:

   .. code-block:: rst

       .. image:: ./media/your_image_file.png
          :align: center
          :alt: Text that is displayed when your image is not available (eg: for screen readers and other accessibility tools)

4. Submit your changes


.. Add a page about a new topic
.. ============================

.. TODO



Technical Details for Nerds
===========================

Advanced users may, of course, fork and clone `the GitHub repository <https://github.com/odoo/documentation-user>`_.
Then submit a pull request with the canonical Git/GitHub workflow.

See our `README <https://github.com/odoo/documentation-user/blob/13.0/README.rst>`_ file about building
the documentation.


Developer documentation
=======================

Documentation that targets developers of Odoo apps is maintained alongside `the source code of Odoo <https://github.com/odoo/odoo/tree/13.0/doc>`_.

.. note::
    User documentation might contain technicalities yet, when they are related to configuration and everyday use of Odoo.



.. |date| date::

*Last revision of this page:* |date|
