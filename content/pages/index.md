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
    height: short
    contentWidth: small
    contentAlignHoriz: center
    contentAlignVert: middle
    bottomGap: none
    topGap: none
    title: Our Services
    text: "Primary Family Care | Telemedicine | Well-Child | Women\x92s Health | Sick Care | Growth Removal | Complete Physicals | DOT Physicals | Sports Physicals | EKGs | Manipulations (OMT) | General Health Issues | Referrals | Pediatric Care | Health Education | Diet Consultation | Diagnosis & Treatment of Acute and Chronic Illness |\_[Immunizations](https://www.cdc.gov/vaccines/schedules/index.html?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fvaccines%2Frecs%2Fschedules%2Fdefault.htm)\_& more...\n"
    styles:
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
  - colors: colors-a
    width: wide
    height: tall
    topGap: medium
    bottomGap: medium
    contentWidth: large
    contentAlignHoriz: left
    contentAlignVert: middle
    elementId: ''
    variant: variant-a
    title: Latest news
    subtitle: Featured blog posts section example
    actions:
      - type: Button
        label: View all
        url: /
        style: primary
    posts:
      - content/pages/blog/post-three.md
      - content/pages/blog/post-two.md
      - content/pages/blog/post-one.md
    type: FeaturedPostsSection
  - colors: colors-a
    width: wide
    height: tall
    topGap: medium
    bottomGap: medium
    contentWidth: large
    contentAlignHoriz: left
    contentAlignVert: middle
    elementId: ''
    variant: variant-a
    title: About us
    subtitle: Meet the team
    actions: []
    people:
      - content/data/team/desmond-eagle.json
      - content/data/team/dianne-ameter.json
      - content/data/team/hilary-ouse.json
    type: FeaturedPeopleSection
  - colors: colors-f
    width: full
    height: short
    topGap: none
    bottomGap: none
    contentWidth: large
    contentAlignHoriz: center
    contentAlignVert: middle
    elementId: ''
    text: |
      ### For appointments and more info please call our office at 509-924-4681
    actions:
      - type: Button
        label: How to Become a Patient
        url: /docs
        style: primary
    actionsPosition: bottom
    type: CtaSection
    styles:
      title:
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
