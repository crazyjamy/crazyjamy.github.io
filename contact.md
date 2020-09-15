---
layout: page
title: Contact
description: Let's talk.
permalink: /contact/
---

<style type="text/css" media="screen">
  .container {
    margin: 0px auto;
    max-width: 600px;
  }
</style>

<div class="container">

  <h2>Talk to me</h2>

  <div id="form" class="contact-form">

<form
  action="https://formspree.io/helllzzzooo@gmail.com"
  method="POST"
>
  <label>
    Your email:
    <input type="text" name="_replyto">
  </label>
  <label>
    Your message:
    <textarea name="message"></textarea>
  </label>

  <!-- your other form fields go here -->

  <button type="submit">Send</button>
</form>
  </div>

</div>
<script src="https://formspree.io/js/formbutton-v1.min.js" defer></script>
<script>
   window.formbutton=window.formbutton||function(){(formbutton.q=formbutton.q||[]).push(arguments)};
   formbutton("create", {action: "https://formspree.io/YOUR_FORM_ID"})
</script>
