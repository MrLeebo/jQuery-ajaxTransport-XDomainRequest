# Cross-Domain AJAX for IE8 and IE9

This fork updates the `XDomainRequest` transport to do a little bit extra.

The request will:
- Send non-GET or POST methods by converting them into a POST and adding the true method in the "_method" parameter
- Copy custom headers (ones starting with X-) as parameters
- Append parameters to the URL for GET requests
