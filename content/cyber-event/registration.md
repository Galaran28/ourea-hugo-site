+++
fragment = "contact"
#disabled = true
date = "2022-04-19"
weight = 1000
background = "dark"
form_name = "register-cyber"

title = "Register for Event"
#subtitle  = "*not working on demo page*"
#title_align = "center" # Default is center, can be left, right or center

# PostURL can be used with backends such as mailout from caddy
#post_url = "https://example.com/mailout" #default: formspree.io
#email = "mail@example.com"
button_text = "Register Space"
netlify = true

# Optional google captcha
# Won't be used if netlify is enabled
#[recaptcha]
#  sitekey = ""

[message]
  success = "Thank you for registering." # defaults to theme default
  error = "Message could not be send. Please contact us at chris@ourea.solutions instead." # defaults to theme default

# Only defined fields are shown in contact form
[fields.name]
  text = "Your Name *"
  error = "Please enter your name" # defaults to theme default

[fields.email]
  text = "Your Email *"
  error = "Please enter your email address" # defaults to theme default

[fields.message]
  text = "Will you be attending in person? And how did you hear about us?"
  error = "Please enter a message"
  required = false

# Optional hidden form fields
# Fields "page" and "site" will be autofilled
[[fields.hidden]]
  name = "page"

+++