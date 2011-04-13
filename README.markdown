# [Mail MIME](http://drupal.org/project/mailmime)

Provides a class for creating MIME messages.

*   *NOTE: This module does not send mail.*

    :   If you came here looking for a mail-sending module, try
        [HTML Mail](http://drupal.org/project/htmlmail) (which can use this
        module for MIME-handling) or
        [Mime Mail](http://drupal.org/project/mimemail) (which comes with its
        own MIME-handling library).

[Mail Mime](http://drupal.org/project/mailmime) extends the
[PEAR](http://pear.php.net/) class called
[Mail_Mime](http://pear.php.net/package/Mail_Mime) to provide a
drupal-friendly library for creating and parsing MIME messages.  Neither
[Mail Mime](http://drupal.org/project/mailmime) nor
[Mail_Mime](http://pear.php.net/package/Mail_Mime) send mail nor do anything
useful on their own.  Both are intended as code libraries to be used by *other*
programs that send or receive mail.

[Mail Mime](http://drupal.org/project/mailmime) started out as part of
[HTML Mail](http://drupal.org/project/htmlmai).  I separated into its own
module for two reasons:

1.  The separation helped clarify in my own mind which parts of the mail-sending
    process require MIME and which do not.  The resulting code is simpler and
    easier to maintain.

2.  It is possible that another mail-sending or mail-reading module may find the
    [Mail Mime](http://drupal.org/project/mailmime) library useful.
