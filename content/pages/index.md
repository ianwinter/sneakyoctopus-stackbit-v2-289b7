---
title: Home
layout: PageLayout
sections:
  - type: HeroSection
    elementId: homepage-hero-1
    colors: colors-a
    title: Helping you untangle the tentacles of technology.
    text: >-
      Aenean eros ipsum, interdum quis dignissim non, sollicitudin vitae nisl.
      Aenean vel aliquet elit, at blandit ipsum. Sed eleifend felis sit amet
      erat molestie, hendrerit malesuada justo ultrices. Nunc volutpat at erat
      vitae interdum. Ut nec massa eget lorem blandit condimentum et at risus.
    actions:
      - label: Let's talk
        altText: Let's talk
        url: /
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        elementId: ''
        type: Link
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-12
          - pr-8
          - pl-8
        alignItems: center
        justifyContent: center
        flexDirection: row
        borderRadius: none
        borderWidth: 0
        borderStyle: none
        borderColor: border-neutral
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: left
        margin:
          - mt-0
          - mb-12
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: left
        margin:
          - mt-0
          - mb-6
      text:
        textAlign: left
        margin:
          - mt-0
          - mb-8
      actions:
        justifyContent: flex-start
  - elementId: quote
    colors: colors-a
    quote: >
      > Talent without discipline is like an octopus on roller skates. There's
      plenty of movement, but you never know if it's going to be forward,
      backwards, or sideways.
    name: 'H. Jackson Brown, Jr.'
    backgroundImage:
      url: ''
      altText: ''
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
          - pl-24
          - pr-24
        alignItems: center
        justifyContent: center
      quote:
        textAlign: left
      name:
        fontWeight: 400
        fontStyle: normal
        textAlign: left
      title:
        fontWeight: 400
        fontStyle: normal
        textAlign: left
    type: QuoteSection
  - type: FeaturedPostsSection
    variant: variant-b
    colors: colors-a
    title: Recent work
    posts:
      - content/pages/blog/post-three.md
      - content/pages/blog/post-two.md
      - content/pages/blog/post-one.md
      - content/pages/blog/post-four.md
      - content/pages/blog/post-five.md
      - content/pages/blog/post-six.md
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-12
          - pr-8
          - pl-8
        justifyContent: center
        borderRadius: none
        borderColor: border-primary
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: center
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: center
        margin:
          - mt-0
          - mb-12
      actions:
        justifyContent: center
    subtitle: Explore case studies
  - elementId: contact-form
    colors: colors-a
    title: Contact me
    text: >
      If you've got a project or want to talk about something, I look forward to
      hearing from you.
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
        - name: message
          label: Message
          placeholder: Tell me about your project or ask a question.
          isRequired: false
          width: full
          type: TextareaFormControl
      submitLabel: Send Message
    feature:
      type: ImageBlock
      url: /images/about.jpg
      altText: Contact us
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        fontWeight: 700
        fontStyle: normal
        textAlign: left
      text:
        textAlign: left
    action: /.netlify/functions/submission_created
    type: ContactSection
---
