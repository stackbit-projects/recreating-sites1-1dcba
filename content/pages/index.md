---
title: Home
layout: PageLayout
sections:
  - type: HeroSection
    elementId: homepage-hero-1
    colors: colors-e
    width: full
    height: tall
    bottomGap: none
    topGap: none
    contentWidth: small
    contentAlignHoriz: center
    contentAlignVert: middle
    text: >
      ## High quality, modern healthcare in a small practice setting. You are
      more than just a number to us. Welcome.
    actions: []
    feature:
      type: ImageBlock
      url: /images/GFP_Clinic_Front_WG_June2021.png
      altText: Gilman Family Practice
    featurePosition: bottom
    styles:
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: center
      actions:
        textAlign: left
  - type: FeaturedPostsSection
    variant: variant-a
    colors: colors-a
    width: full
    height: short
    contentWidth: medium
    contentAlignHoriz: center
    contentAlignVert: middle
    bottomGap: none
    topGap: none
    posts:
      - content/pages/blog/post-three.md
      - content/pages/blog/post-two.md
      - content/pages/blog/post-one.md
    styles:
      title:
        textAlign: center
      subtitle:
        textAlign: center
      actions:
        textAlign: center
  - type: TextSection
    colors: colors-f
    width: full
    height: tall
    contentWidth: small
    contentAlignHoriz: center
    contentAlignVert: middle
    bottomGap: none
    topGap: none
    title: Our Services
    subtitle: The section subtitle
    text: >-
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam. Eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
      Sed ut perspiciatis undeomnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam. Eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
    styles:
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
  - type: ContactSection
    variant: variant-b
    colors: colors-h
    width: wide
    height: tall
    title: Join our club
    bottomGap: none
    topGap: none
    text: >-
      We will notify you every time a shipment is heading to your neighborhood,
      and you could immediatly let us know if you want in or not.
    feature:
      type: ImageBlock
      url: /images/contact.png
      altText: Fisherman holding lobster
    form:
      type: FormBlock
      elementId: contact-form
      destination: ''
      action: /.netlify/functions/submission_created
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
    styles:
      title:
        textAlign: left
      text:
        textAlign: left
---
