---
layout: page
title: "Contact Me"
permalink: /contact/
show_excerpts: false
---
<div>
<center>
  <p>Send me an email at 
    <a href="mailto:hello@susangfink.com">hello@susangfink.com</a> or use the form below</p>
</center>
</div>

<div id="formkeep-embed" data-formkeep-url="https://formkeep.com/p/eb5735959c0e93a89110b274fcc0cc4b?embedded=1"></div>

<script type="text/javascript" src="https://pym.nprapps.org/pym.v1.min.js"></script>
<script type="text/javascript" src="https://cdn.formkeep.com/formkeep-embed.js"></script>

<!-- Get notified when the form is submitted, add your own code below: -->
<script>
const formkeepEmbed = document.querySelector('#formkeep-embed')

formkeepEmbed.addEventListener('formkeep-embed:submitting', _event => {
  console.log('Submitting form...')
})

formkeepEmbed.addEventListener('formkeep-embed:submitted', _event => {
  console.log('Submitted form...')
})
</script>
