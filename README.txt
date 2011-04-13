                                  [1]Mail MIME

   Provides a class for creating MIME messages.
     *

        NOTE: This module does not send mail.
                If you came here looking for a mail-sending module, try
                [2]HTML Mail (which can use this module for MIME-handling)
                or [3]Mime Mail (which comes with its own MIME-handling
                library).

   [4]Mail Mime extends the [5]PEAR class called [6]Mail_Mime to provide a
   drupal-friendly library for creating and parsing MIME messages. Neither
   [7]Mail Mime nor [8]Mail_Mime send mail nor do anything useful on their
   own. Both are intended as code libraries to be used by other programs
   that send or receive mail.

   [9]Mail Mime started out as part of [10]HTML Mail. I separated into its
   own module for two reasons:
    1. The separation helped clarify in my own mind which parts of the
       mail-sending process required MIME and which did not. The resulting
       code is simpler and easier to maintain.
    2. It is possible that another mail-sending or mail-reading module may
       find the [11]Mail Mime library useful.

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
