---
layout: page
title: "Contact Me"
permalink: /contact/
show_excerpts: false
---

<div>
<center>
  <p>Follow me on Instagram 
    <a href="http://www.instagram.com/susanfink">@susanfink</a> </p>
</center>
</div>
<div>
<center>
  <p>Send me an email at 
    <a href="mailto:hello@susangfink.com">hello@susangfink.com</a> or use the form below</p>
</center>
</div>


<form
  action="https://formspree.io/f/xgoebyya"
  method="POST"
  class="contact-form"
  id="contact-form"
>
  <p align="left">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" required>
    
  </p>

  <p>
    <label for="email">Email</label>
      <input type="email" id="email" name="email" required>
  </p>

  <p>
    <label for="message">Message</label>
      <textarea id="message" name="message" rows="6" required></textarea>
  </p>

  <p>
    <button type="submit" class="btn">Send Message</button>
  </p>
</form>

<center>
  <p id="form-success" class="form-success" hidden>
  Thank you! Your message has been sent.
</p>
</center>

<script>
  const form = document.getElementById('contact-form');
  const successMessage = document.getElementById('form-success');

  form.addEventListener('submit', async function (e) {
    e.preventDefault();

    const formData = new FormData(form);

    const response = await fetch(form.action, {
      method: form.method,
      body: formData,
      headers: {
        'Accept': 'application/json'
      }
    });

    if (response.ok) {
      form.reset();
      form.style.display = 'none';
      successMessage.hidden = false;
    }
  });
</script>
