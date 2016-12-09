---
layout: page
title: "Contact"
# meta_title:
#subheadline:
teaser: "Need to get in touch with me? Use the contact form."
header:
   image_fullwidth: "airplane.jpg"
permalink: "/contact/"
---

<form action="https://getsimpleform.com/messages?form_api_token=d13749883e17be136984e5a03c1b5cd3" method="post" onSubmit="javascript: return confirm('Are you sure you want to submit this?');">
    <!-- the redirect_to is optional, the form will redirect to the referrer on submission -->
    <!-- <input type='hidden' name='redirect_to' value='<the complete return url e.g. http://fooey.com/thank-you.html>' /> -->
    <!-- all your input fields here.... -->
    <div class="form-group">
        <label for="InputName1">Your Name</label>
        <input type="text" class="form-control" name="name">
    </div>
    <div class="form-group">
        <label for="InputEmail1">Email Address</label>
        <input type="email" class="form-control" name="email">
    </div>
    <div class="form-group">
        <label for="InputSubject1">Subject</label>
        <input type="text" class="form-control" name="subject">
    </div>
    <div class="form-group">
        <label for="message1">Message</label>
        <textarea class="form-control" name="message" rows="3"></textarea>
    </div>
    <input type='submit' value='Submit' />             
</form>
