---
title: "Contact Me"
layout: page
permalink: /contact/
show_excerpts: false
---
<div>
<p>Send me an email at hello@susangfink.com or use the form below</p>
</div>
<div id="formkeep-embed" data-formkeep-url="https://formkeep.com/p/eb5735959c0e93a89110b274fcc0cc4b"></div>

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
