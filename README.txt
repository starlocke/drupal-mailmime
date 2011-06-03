[1]Mail MIME

   Provides a class for creating MIME messages.
     *

        NOTE: This module does not send mail.
                If you came here looking for a mail-sending module, try
                [2]HTML Mail (which can use this module for MIME-handling)
                or [3]Mime Mail (which comes with its own MIME-handling
                library).

   [4]Mail Mime extends the [5]PEAR class called [6]Mail_Mime (version
   1.6.1 or later) to provide a drupal-friendly library for creating and
   parsing MIME messages. Neither [7]Mail Mime nor [8]Mail_Mime send mail
   nor do anything useful on their own. Both are intended as code
   libraries to be used by other programs that send or receive mail.

   [9]Mail Mime started out as part of [10]HTML Mail. I separated into its
   own module for two reasons:
    1. The separation helped clarify in my own mind which parts of the
       mail-sending process require MIME and which do not. The resulting
       code is simpler and easier to maintain.
    2. It is possible that another mail-sending or mail-reading module may
       find the [11]Mail Mime library useful.

  [12]Requirement

   The following files, available from [13]PEAR, must be installed and
   available somewhere on the [14]include_path.
     * Mail/mime.php
     * Mail/mimeDecode.php
     * Mail/mimePart.php
     * PEAR.php
     * PEAR5.php

   One way to satisfy this requirement is to run the following command
   from a Unix root shell prompt:
pear install -a Mail_Mime


   Another way is to install and enable the [15]Include module before
   enabling the [16]Mail MIME module.

  [17]Installation

    1. Download and install [18]as usual.
    2. When enabled, [19]Mail Mime will
          + Auto-detect whether the required files are present.
          + If any files are missing, and the [20]Include module is
            available, [21]Mail Mime will use [22]Include to auto-download
            and enable the missing files.
          + If all of the above fails, [23]Mail Mime will disable itself
            and print a warning to both the screen and the error log.

References

   1. http://drupal.org/project/mailmime
   2. http://drupal.org/project/htmlmail
   3. http://drupal.org/project/mimemail
   4. http://drupal.org/project/mailmime
   5. http://pear.php.net/
   6. http://pear.php.net/package/Mail_Mime
   7. http://drupal.org/project/mailmime
   8. http://pear.php.net/package/Mail_Mime
   9. http://drupal.org/project/mailmime
  10. http://drupal.org/project/htmlmai
  11. http://drupal.org/project/mailmime
  12. http://www.dict.org/bin/Dict?Form=Dict2&Database=*&Query=requirement
  13. http://pear.php.net/
  14. http://php.net/manual/ini.core.php#ini.include-path
  15. http://drupal.org/project/include
  16. http://drupal.org/project/mailmime
  17. http://drupal.org/documentation/install/modules-themes/modules-5-6
  18. http://drupal.org/documentation/install/modules-themes/modules-5-6
  19. http://drupal.org/project/mailmime
  20. http://drupal.org/project/include
  21. http://drupal.org/project/mailmime
  22. http://drupal.org/project/include
  23. http://drupal.org/project/mailmime
