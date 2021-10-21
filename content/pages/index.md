---
title: Home
layout: PageLayout
sections:
  - elementId: contact-form
    colors: colors-c
    width: full
    height: short
    contentWidth: large
    contentAlignHoriz: center
    contentAlignVert: middle
    topGap: none
    bottomGap: none
    variant: variant-b
    title: Contact us
    text: We look forward to hearing from you.
    form:
      type: FormBlock
      elementId: contact-form
      action: /.netlify/functions/submission_created
      destination: ''
      fields:
        - type: TextFormControl
          name: name
          label: Name
          placeholder: Your name
          isRequired: true
          width: 1/2
        - type: EmailFormControl
          name: email
          label: Email
          placeholder: Your email
          isRequired: true
          width: 1/2
        - type: TextFormControl
          name: home-address
          label: Home address
          placeholder: Your home address
          isRequired: true
          width: full
        - type: CheckboxFormControl
          name: updates
          label: Sign me up to receive updates
          width: full
      submitLabel: Send Message
    feature:
      type: ImageBlock
      url: /images/contact.png
      altText: Contact form image
    action: /.netlify/functions/submission_created
    type: ContactSection
  - elementId: ''
    colors: colors-a
    width: wide
    height: short
    contentWidth: large
    contentAlignHoriz: center
    contentAlignVert: middle
    topGap: none
    bottomGap: none
    variant: variant-b
    title: Testimonials
    subtitle: What our customers say about us
    testimonials:
      - type: Testimonial
        quote: >-
          “It’s great to see someone taking action while still maintaining a
          sustainable fish supply to home cooks.”
        name: Johnna Doe
        title: Product Marketing Manager at Acme
        image:
          type: ImageBlock
          url: /images/dianne-ameter.jpg
          altText: Product Marketing Manager
    type: TestimonialsSection
  - type: HeroSection
    title: Stackbit Starter
    text: >-
      The Stackbit Nextjs Starter is intended to be used with a theme from
      https://github.com/stackbit-themes
---
