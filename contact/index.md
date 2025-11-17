---
layout: page
title: Contact
eyebrow: Get in touch
subtitle: Use the form below or write to computeel@usp.br.
hero_image: /assets/images/hero-default.jpg
hero_tags:
  - Collaborations
  - Undergraduate research
  - Graduate positions
---

Need to reach ComputEEL/MatSci? Send a message through the form or write directly to [{{ site.email }}](mailto:{{ site.email }}). We’ll get back to you as soon as possible.

<div class="card" style="max-width:720px; margin:1rem auto;">
  <form action="https://formspree.io/f/mbjpvrvd" method="POST" class="contact-form">
    <label>Email*</label>
    <input type="email" name="email" required placeholder="you@example.com">
    <label>Message*</label>
    <textarea name="content" rows="6" required placeholder="Your message"></textarea>
    <button class="nav-cta" type="submit" style="border:0;">Send</button>
  </form>
</div>

<style>
.contact-form {
  display: grid;
  gap: 0.75rem;
}
.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 0.75rem;
  border-radius: 10px;
  border: 1px solid rgba(12,43,67,0.15);
  font-family: 'Inter', system-ui;
}
</style>
