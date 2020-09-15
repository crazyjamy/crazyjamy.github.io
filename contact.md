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
    <form accept-charset="UTF-8" method="POST" action="https://formspree.io/{{ site.email }}" v-on:submit.prevent="validateBeforeSubmit" ref="contact">
      <fieldset>
        <input type="hidden" name="_subject" value="New contact!" />
        <input type="hidden" name="_next" value="{{ site.url }}/contact/message-sent/" />
        <input type="hidden" name="_language" value="en" />

        <input type="text" name="name" placeholder="이름이 뭐에요? 😶" v-validate="'required'"
               :class="{ 'has-error': errors.has('name') }">
        <span v-if="errors.has('name')" v-cloak>${ errors.first('name') }</span>

        <input type="text" name="email" placeholder="이메일은요? 👀" v-validate="'required|email'"
               :class="{ 'has-error': errors.has('email') }">
        <span v-if="errors.has('email')" v-cloak>${ errors.first('email') }</span>

        <textarea name="message" onkeyup="adjust_textarea(this)" placeholder="하시고 싶은 말을 적어주세요. 📝 보내기 후 확인 페이지로 넘어갑니다. 최종 확인하셔야 메일이 보내집니다. " v-validate="'required'"
                  :class="{ 'has-error': errors.has('message') }"></textarea>
        <span v-if="errors.has('message')" v-cloak>${ errors.first('message') }</span>

        <button type="submit">보내기</button>
      </fieldset>
    </form>
  </div>

</div>
<script src="https://formspree.io/js/formbutton-v1.min.js" defer></script>
<script>
   window.formbutton=window.formbutton||function(){(formbutton.q=formbutton.q||[]).push(arguments)};
   formbutton("create", {action: "https://formspree.io/YOUR_FORM_ID"})
</script>
