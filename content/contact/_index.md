---
layout: simple
---

</br></br>

# Get In Touch

<h3>Feel free to reach out to me through any of these channels.</h3>

<div class="contact-grid">
  <!-- Email -->
  <div class="contact-card">
    <div class="contact-icon">
      {{< icon "email" >}}
    </div>
    <div class="contact-info">
      <h3>Email</h3>
      <a href="mailto:zizovic.aleksandar@outlook.com">zizovic.aleksandar@outlook.com</a>
    </div>
  </div>
  
  <!-- LinkedIn -->
  <div class="contact-card">
    <div class="contact-icon">
      {{< icon "linkedin" >}}
    </div>
    <div class="contact-info">
      <h3>LinkedIn</h3>
      <a href="https://linkedin.com/in/aleksandar-zizovic" target="_blank">linkedin.com/in/aleksandar-zizovic</a>
    </div>
  </div>
  
  <!-- GitHub -->
  <div class="contact-card">
    <div class="contact-icon">
      {{< icon "github" >}}
    </div>
    <div class="contact-info">
      <h3>GitHub</h3>
      <a href="https://github.com/z1z0v1c" target="_blank">github.com/z1z0v1c</a>
    </div>
  </div>
  
  <!-- Twitter -->
  <div class="contact-card">
    <div class="contact-icon">
      {{< icon "twitter" >}}
    </div>
    <div class="contact-info">
      <h3>Twitter</h3>
      <a href="https://twitter.com/z1z0v1c" target="_blank">@z1z0v1c</a>
    </div>
  </div>
</div>

</br></br>

# Where am I? 

<div class="contact-grid">
<!-- Location -->
  <div class="contact-card">
    <div class="contact-icon">
      {{< icon "location-dot" >}}
    </div>
    <div class="contact-info">
      <p>Belgrade, Serbia</p>
    </div>
  </div>
</div>

<style>
.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.contact-card {
  display: flex;
  align-items: flex-start;
  padding: 1.5rem;
  border-radius: 8px;
  background-color: var(--ifm-card-background-color);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s, box-shadow 0.2s;
}

.contact-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
}

.contact-icon {
  margin-right: 1rem;
  color: var(--ifm-color-primary);
  font-size: 1.5rem;
}

.contact-info h3 {
  margin-top: 0;
  margin-bottom: 0.5rem;
}

.contact-info a {
  color: var(--ifm-color-primary);
  text-decoration: none;
}

.contact-info a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .contact-grid {
    grid-template-columns: 1fr;
  }
}
</style>

</br></br>

# Send Me a Message

<form action="https://formspree.io/f/xgvapgqn" method="POST" id="contact-form">
  <div class="form-row">
    <label for="name">Name</label>
    <input type="text" name="name" id="name" required>
  </div>
  
  <div class="form-row">
    <label for="email">Email</label>
    <input type="email" name="email" id="email" required>
  </div>
  
  <div class="form-row">
    <label for="subject">Subject</label>
    <input type="text" name="subject" id="subject" required>
  </div>
  
  <div class="form-row">
    <label for="message">Message</label>
    <textarea name="message" id="message" rows="4" required></textarea>
  </div>
  
  <button class="btn" type="submit">Send Message</button>
</form>

<!-- <script>
  document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault();
    
    const form = event.target;
    const formData = new FormData(form);
    
    fetch(form.action, {
      method: 'POST',
      body: formData,
      headers: {
        'Accept': 'application/json'
      }
    })
    .then(response => {
      if (response.ok) {
        form.reset();
        alert('Thank you for your message! I will get back to you soon.');
      } else {
        alert('Oops! There was a problem submitting your form. Please try again.');
      }
    })
    .catch(error => {
      alert('Oops! There was a problem submitting your form. Please try again.');
    });
  });
</script> -->

<style>
  #contact-form {
    max-width: 100%;
    margin: 2rem 0;
  }
  
  .form-row {
    margin-bottom: 1rem;
  }
  
  label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 500;
  }
  
  input, textarea {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 1rem;
  }
  
  .btn {
    background-color: #3b82f6;
    color: white;
    border: none;
    padding: 0.75rem 1.5rem;
    border-radius: 4px;
    font-size: 1rem;
    cursor: pointer;
    margin-top: 1rem;
  }
  
  button:hover {
    background-color: #2563eb;
  }
</style>