
ChangeLog
==============================================================================

All bugs/feature details can be found at: 

   https://github.com/derks/drest/issues/XXXXX


Where XXXXX is the 'Issue #' referenced below.  Additionally, this change log
is available online at:

    http://drest.readthedocs.org/en/latest/changelog.html

.. raw:: html

    <BR><BR>

0.9.7 - Development version (will be released as 0.9.8)
------------------------------------------------------------------------------

Bug Fixes:

    * :issue:`12` - Params are not added correctly to GET request
    
Feature Enhancements:

    None
    

0.9.6 - Mar 23, 2012 
------------------------------------------------------------------------------

Bug Fixes:

    - :issue:`9` - GET params incorrectly stored as permanent 
      _extra_url_params.
 
Feature Enhancements:

    - :issue:`4` - Better support for nested resource names.
    - :issue:`5`, :issue:`8` - Request object is now exposed publicly.
    - :issue:`6` - Add capability to suppress final forward-slash
    - :issue:`7` - Cache http object for improved performance.
    
Incompatible Changes:

    - api._request is now api.request.  api.request (old function) is now
      api.make_request()
    
    - Lots of code refactoring.. numerous minor changes may break 
      compatibility if using backend functions, but not likely if accessing
      the high level api functions.
    
    - Every request now returns a drest.response.ResponseHandler object 
      rather than a (response, data) tuple.  
      
      
0.9.4 - Feb 16, 2012
------------------------------------------------------------------------------

Bug Fixes:

    - :issue:`3` - TypeError: object.__init__() takes no parameters
 
Feature Enhancements:

    - Improved test suite, now powered by Django TastyPie!
    - Added support for Basic HTTP Auth.
    
Incompatible Changes:

    - drest.api.API.auth() now implements Basic HTTP Auth by default rather
      than just appending the user/password/etc to the URL.
    
    
.. raw:: html

    <BR><BR>
    
0.9.2 - Feb 01, 2012
------------------------------------------------------------------------------

    - Initial Beta release.  Future versions will detail bugs/features/etc.