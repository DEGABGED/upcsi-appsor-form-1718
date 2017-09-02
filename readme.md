# Description
This small webpage supposedly serves as a frontend to a Google Form. The form in the HTML will post the data to the Google Form. So far, the redirect is still not done.

# Issues
While the posting of data works, the page still redirected to the Google Form finish page. A proposed fix here was to submit the data via AJAX and use a callback to stop the redirect. However, this resulted in an error: "No 'Access-Control-Allow-Origin' header is present on the requested resource. Origin 'null' is therefore not allowed access.". This error stopped following JS that handled the form submission pop-up and reset. Weirdly enough, however, the data was still submitted.

The responses for both the original form (where it redirected to the Google Form finish page) and the AJAX-submitted form (with the error) are both in this repository as `response-post.txt` and `response-ajax.txt`, respectively. Screenshots can also be found at `images/`.
